# serbian_pyspark

The Serbian Web Corpus (srWaC) contains nearly a billion tokens scraped from .rs domains. Each word is lemmatized and characterized with linguistic properties to save computation time. 

In this project we lightly parse these xml records to mine for sentences which contained possessive pronouns, which vary in declension by the case, gender, and number of the noun involved. Spark speeds up this process by naturally involving all cores of a local computer and enabling even faster distributed processing in a cluster.

In practice, some usages are much less common than others and some inappropriate sentences are removed. Results are shown below for njegov- in which the owned object is neuter gender singular, in the nominative case.

{'lemma': 'njegov', 'Case': 'Nom', 'Gender': 'Neut', 'Number': 'Sing'}

Serbian:  
To je njegovo Ustavom zagarantovano pravo.  
Ipak, njegovo izručenje će biti uslov  
Njegovo Preosveštenstvo Mitropolit Konstantin se trenutno nalazi  
Bez njegovo znanje nema godižbina trošenje.  
Roditelj može da smatra da je njegovo  
I zato njegovo ponašanje smatram nekorektnim.  
Njegovo preduzeće najveći deo prometa ostvaruje preko  
Jos kada bi se na izborima njegovo  
Na pitanje kakvo je bilo njegovo reagovanje  
Brižno odabiranje kamena i njegovo samo delimično  
Njegovo Preosveštenstvo Episkop zvorničko-tuzlanski G.  
Njegovo delovanje na državnim funkcijama je,  
Njegovo Preosveštenstvo Episkop hvostanski G.  
Njegovo ime nalazi se na spisku među  
Uz njegovo zdušno zalaganje, te nekoliko  
Njegovo Preosveštenstvo Episkop hvostanski Atanasije u nadahnutoj  
Irineja, Njegovo Preosveštenstvo Episkop šabački g.  
Pri pogledu na publiku njegovo divljenje je  
Njegovo igrano ostvarenje" Gegen die Wand  
Nema sumnje da njegovo sitno seme i  


English auto-translation:  
That is his right guaranteed by the Constitution.  
However, his extradition will be a condition  
His Eminence Metropolitan Constantine is currently present  
Without his knowledge there is no anniversary of spending.  
The parent may consider it his  
And that is why I consider his behavior incorrect.  
His company generates most of its turnover through  
Even if it were his election  
When asked what his reaction was  
Careful selection of stone and its only partial  
His Eminence Bishop of Zvornik-Tuzla G.  
His work in state functions is,  
His Eminence Bishop Hvostanski G.  
His name is on the list among  
With his heartfelt commitment, and a few  
His Eminence Bishop Atanasije of Hvostan was inspired  
Irinej, His Eminence Bishop of Sabac Mr.  
Looking at the audience is his admiration  
His feature film “Gegen die Wand  
There is no doubt that his tiny seeds and  
