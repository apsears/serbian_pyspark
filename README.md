# serbian_pyspark

The Serbian Web Corpus: [srWaC](http://nlp.ffzg.hr/resources/corpora/srwac/) contains nearly a billion tokens in the Serbo-Croatian language scraped from .rs domains. Each word is lemmatized and characterized with linguistic properties to save computation time. 

In this project we lightly parse these xml records to mine for sentences which contain possessive pronouns, which vary in declension by the case, gender, and number of the noun involved. Spark speeds up this process by naturally involving all cores of a local computer and enabling even faster distributed processing in a cluster.

In practice, some usages are much less common than others and some inappropriate sentences are removed. Results are shown below for the third-person possessive pronoun njegov- for the nominative case, and in which the owned object is neuter gender singular.

{'lemma': 'njegov', 'Case': 'Nom', 'Gender': 'Neut', 'Number': 'Sing'}

Serbian:  
1. To je njegovo Ustavom zagarantovano pravo.  
2. Ipak, njegovo izručenje će biti uslov  
3. Njegovo Preosveštenstvo Mitropolit Konstantin se trenutno nalazi  
4. Bez njegovo znanje nema godižbina trošenje.  
5. Roditelj može da smatra da je njegovo  
6. I zato njegovo ponašanje smatram nekorektnim.  
7. Njegovo preduzeće najveći deo prometa ostvaruje preko  
8. Jos kada bi se na izborima njegovo  
9. Na pitanje kakvo je bilo njegovo reagovanje  
10. Brižno odabiranje kamena i njegovo samo delimično  
11. Njegovo Preosveštenstvo Episkop zvorničko-tuzlanski G.  
12. Njegovo delovanje na državnim funkcijama je,  
13. Njegovo Preosveštenstvo Episkop hvostanski G.  
14. Njegovo ime nalazi se na spisku među  
15. Uz njegovo zdušno zalaganje, te nekoliko  
16. Njegovo Preosveštenstvo Episkop hvostanski Atanasije u nadahnutoj  
17. Irineja, Njegovo Preosveštenstvo Episkop šabački g.  
18. Pri pogledu na publiku njegovo divljenje je  
19. Njegovo igrano ostvarenje" Gegen die Wand  
20. Nema sumnje da njegovo sitno seme i  


English auto-translation:  
1. That is his right guaranteed by the Constitution.  
2. However, his extradition will be a condition  
3. His Eminence Metropolitan Constantine is currently present  
4. Without his knowledge there is no anniversary of spending.  
5. The parent may consider it his  
6. And that is why I consider his behavior incorrect.  
7. His company generates most of its turnover through  
8. Even if it were his election  
9. When asked what his reaction was  
10. Careful selection of stone and its only partial  
11. His Eminence Bishop of Zvornik-Tuzla G.  
12. His work in state functions is,  
13. His Eminence Bishop Hvostanski G.  
14. His name is on the list among  
15. With his heartfelt commitment, and a few  
16. His Eminence Bishop Atanasije of Hvostan was inspired  
17. Irinej, His Eminence Bishop of Sabac Mr.  
18. Looking at the audience is his admiration  
19. His feature film “Gegen die Wand  
20. There is no doubt that his tiny seeds and  
