# BlogSpot-Metadata-Template
Blogspot template with Schema microdata modifications

A BlogSpot (Google Blogger) template modified to eliminate Schema.org errors when testing with Google's Structured Data Testing Tool (SDTT) as of January 29, 2016.

This is a standard "Simple" Template created by Designer: Josh Peterson (URL:www.noaesthetic.com), which seems to retain all of the functionality of the "Blogger Template Designer".

Intended for those wishing to start a new Blogger blog. 

*** WARNING: Installing over an existing blog will destroy your existing layout and other preferences. 

<h3>Customizations:</h3>

The Template works as is, however you should provide your own images.

<b>There are two locations in the Template for the two images required by Google's (SDTT).</b>
```
<!--  Schema Mods:Provide your image urls and sizes here -->
  <!-- Image for the blogposting -->  
              <meta itemprop='url' content='full-url-to.YOUR-BLOG'S-IMAGE.png'/>
              <meta itemprop='width' content='800'/>
              <meta itemprop='height' content='800'/>
            </div>
            
            <div itemprop='publisher' itemscope='itemscope' itemtype='https://schema.org/Organization'>
              <div itemprop='logo' itemscope='itemscope' itemtype='https://schema.org/ImageObject'>
  <!--Image for the Organization --> 
                <img style='display:none;' src='full-url-to.YOUR-ORGANIZATION'S-IMAGE.png'/>
                <meta itemprop='url' content='full-url-to.YOUR-ORGANIZATION'S-IMAGE.png'/>
                <meta itemprop='width' content='600'/>
                <meta itemprop='height' content='60'/>
              </div>
            <meta itemprop='name' expr:content='data:blog.title'/>
            </div>
          </div>
<!--  Schema Mods:End -->

```
Search the within the template for "Schema Mods:" to locate those areas and provide your images.
(Dummy images are currently in those sections for testing.)

<b>There is also a commented area in the <Head> section for providing your Google Plus identity.</b>
```
<!--  Schema Mods: Code to provide Google+ account programatically (for removal of "About Me" gadget)
   <link rel='Author' href='http://plus.google.com/xxxxxxxxxxxxxxxxxxxxx'/>
   <link rel='Publisher' href='http://plus.google.com/xxxxxxxxxxxxxxxxxxxxx'/>
-->
```
Just provide your Google+ id in the place of the xxxxxxxxxxxxxxxxxxxxx and uncomment.

<h3>Resources</h3>

Hat Tip to Technohalf for sharing a tutorial with mostly correct information at:<br/> http://www.technohalf.com/2015/12/how-to-fix-all-structured-data-errors.html?showComment=1454110555230#c3338431680769504293

Google's Structured Data Testing Tool:<br/>
https://developers.google.com/structured-data/testing-tool/

Google's Rich Snipets for Articles:<br/>
https://developers.google.com/structured-data/rich-snippets/articles

Schema.org: Article<br/>
https://schema.org/Article
