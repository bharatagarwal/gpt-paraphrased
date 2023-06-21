Working off this blog post:
https://developers.googleblog.com/2008/07/protocol-buffers-our-serialized.html

and the video introduced subsequently:
https://www.youtube.com/watch?v=K-e8DDRwVUg

-------

Today, we have something quite intriguing to present to you.

Could you, Kenton, begin by introducing yourself to our audience?

My name is Kenton Varda, and I serve as an engineer in this esteemed place.

Fantastic. Could you please enlighten us about the product you've released today?

What we've released is named Protocol Buffers, and it's essentially the methodology we apply for encoding structured data here at Google.

Let me attempt to illustrate the core concept. First, you compose a 'proto' file that embodies the definitions of structured data. Subsequently, this file is processed via the protocol compiler, which generates relevant classes in C++, Java or Python, representing the structures you have defined.

Each of these classes incorporates accessors for all the fields you've defined and contains methods for parsing and serializing the data in a compact and swift format. This format is ubiquitous in our data interchange processes at Google.

It's fascinating to note that when most people contemplate structured data, XML comes to mind.

What led to the non-usage of XML and the adoption of this new structure?

XML has its merits, however, due to the colossal volume of data we manage here, it was found to be inadequate. XML's encoding and decoding process is time-consuming and its size is somewhat bulky. We required an exceedingly efficient system.

The secondary issue lies in the fact that XML, contingent upon the kind of data you are trying to represent, can be fairly clunky. For instance, if you aim to represent something akin to HTML, which is essentially text with markup, then XML is ideal. However, if you're representing data structures with a simple set of fields, XML becomes cumbersome due to the need to navigate this DOM tree and parse elements.

So this data is typed, then?

Correct. Protocol Buffers are robustly typed.

People often draw parallels between IDL, CORBA and Protocol Buffers. Do you believe this is a valid comparison?

Every system possesses unique strengths and weaknesses. Protocol Buffers merely offers a method for data encoding and isn't an RPC system per se. Although, it can be employed for RPC, and indeed, we do use it for that purpose. This release does not comprise any form of RPC implementation. Instead, it's crafted to be used with any RPC implementation that one desires.

Could you elucidate the historical development of Protocol Buffers?

It's a narrative that spans some years. Protocol Buffers initially emerged, I believe, in the late stages of a particular year. During this period, I was not a part of Google, however, Jeff Dean and Sanjay Ghemawat, who were responsible for significant technologies like MapReduce and BigTable, are credited with its inception.

In its primary form, you could define proto files which then generated a set of numerical constants. These constants were used to manually write parsers and encoders for various formats. Over time, it evolved to the stage where the protocol compiler automatically generates everything.

So, as an end user developer, you receive a Java class which you can manipulate. Essentially, it uses GET to retrieve various data and SET to input data into the system, functioning at a lower level with binary files.

Precisely. You simply create your message class and utilize the SET "whatever" accessors to set each field. Following this, you serialize the string or serialize to an output stream.

As Protocol Buffers is now open source and accessible for experimentation, what do you foresee as its potential uses in contrast to other solutions? Where does it truly excel?

Primarily, if you require a swift, compact format that's easy to define and extendable, meaning you can modify fields while still maintaining compatibility with older programs using the previous version of the format, Protocol Buffers are an excellent solution. However, they may not be ideal for representing structured text because they're not a text format and structured text can't be easily inserted. They might also fall short if human readability is your foremost priority since, while there is a text format for debugging, Protocol Buffers is primarily a binary format.

You spoke of manipulating data, is there any sort of built-in schema versioning?

Yes, indeed. When you add new fields to your structures and then encode a message using these new fields, older programs not aware of them will simply disregard them. If you remove a field, older programs will assume it has its default value. 

It's a remarkable feature, indeed. Not having to fiddle with schemas and navigate through intricate systems if it's all built into the protocol itself seems highly beneficial.

Do you have any final thoughts or advice for developers who are having their first glance at this open source package?

Indeed, I encourage everyone to examine the documentation, download the code which is freely available, and share your thoughts on our discussion group.

Well, thank you so much for your efforts in bringing this to fruition. I know many who have departed from Google and wished they had Protocol Buffers at their disposal. It's certainly exciting to see it out in the wild now, and we greatly appreciate it.
