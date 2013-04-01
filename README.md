NFArrayToXml
============

Simple conversion of an array to XML and back again.

This is a wrapper around Lalit Patel's [Array2XML][1] & [Xml2Array][2]


Installation
------------

Using [Composer](http://getcomposer.org):

    {
        "repositories": [
            {
                "type": "vcs",
                "url": "https://github.com/nineteenfeet/NFArrayToXml"
            }
        ],
        "require": {
            "nineteenfeet/nf-array-to-xml": "1.*",
        }
    }

Alternatively, install manually.

Usage
-----

Array to XML: 

    $xml = \NFArrayToXml\ArrayToXml::createXML('root_node_name', $array);
    echo $xml->saveXML();

XML to array:

    $array = \NFArrayToXml\XmlToArray::createArray($xml);



[1]: http://www.lalit.org/wordpress/wp-content/uploads/2011/07/Array2XML.txt
[2]: http://www.lalit.org/wordpress/wp-content/uploads/2011/07/XML2Array.txt
