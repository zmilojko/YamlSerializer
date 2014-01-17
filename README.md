# YamlSerializer 

This is a YAML (de)serializer for .NET.

You can do something like this with it:

        System.Yaml.Serialization.YamlSerializer ser = new System.Yaml.Serialization.YamlSerializer();
        MySerializableClass obj = (MySerializableClass)ser.DeserializeFromFile(filepath, typeof(MySerializableClass))[0];

and then something like this:

        ser.SerializeToFile(filepath, obj);

And of course, it can also serialize to and from strings. (Note that it can 
serialize multiple objects from a same source, this the [0] in the end of the 
first example.)

## History

Searching for a simple YAML serializer, I run into this deserted project,
which was stored using Mercurial on CodePlex. It almost worked out of the box,
but for the almost part I needed to make some changes.

Not being too eager to start installing such dead tools as mercurial or 
registering to even deader sites, decided to take only what I need and move
it to Git and GitHub.

Any kudos is due to the original author, Osamu Takeuchi.

Original web page:

	http://yamlserializer.codeplex.com/

License:
	YamlSerializer is distributed under the MIT license as following:

---
The MIT License (MIT)

Changes: Copyright (c) 2013 Zeljko Milojkovic <zeljko@zwr.fi>

Original code: Copyright (c) 2009 Osamu TAKEUCHI <osamu@big.jp>

Permission is hereby granted, free of charge, to any person obtaining a copy of 
this software and associated documentation files (the "Software"), to deal in the 
Software without restriction, including without limitation the rights to use, copy, 
modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
and to permit persons to whom the Software is furnished to do so, subject to the 
following conditions:

The above copyright notice and this permission notice shall be included in all 
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A 
PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT 
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF 
CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE 
OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
