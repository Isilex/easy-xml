---
layout: page
title: TroubleShooting
---

<div class="texteLong" lang="en">
            
              <div> <div> <div> <p>
                      <strong>- &nbsp;I get a 503 error message :</strong>
                    </p> <p>It's a Java problem. You just need to download again an Isilex Zip Archive, with "no Java" included.</p> <p>
                      <strong>- I uploaded a new XML Corpus in IsiCorpus, but it stops:</strong>
                    </p> <p>IsiCorpus is made for those who wants to use XML without learning how to build a structure: you can only upload .txt files. If you already have an XML Corpus, you just need to create a new database and insert it into "data" directory, therefore you just have to write your own XQuery Rest WebPage into Addiotional.xqm file into "webapp" directory. Here is a very simple one you can use to display your entire corpus into an Isilex Webpage:</p> <pre>1. declare %rest:path('/monAppli') <br clear="none">2. %output:method('xhtml') <br clear="none">3. function isilex:monAppli()<br clear="none">4. { <br clear="none">5. isi:template<br clear="none">6. ( for $x in db:open('[MASUPERBASE]')/[ROOT] return $x ) <br clear="none">7. }; </pre> </div> </div> </div>
            
          </div>