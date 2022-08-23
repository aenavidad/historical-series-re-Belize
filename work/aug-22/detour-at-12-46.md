# detour-at-12-46

## abstract

this file contains output from step 50 of [[extractions.md]][^file written 22 aug 2022 12.48 in Boston MA.]

## current content

this section contains full extracts of all content within files listed in step 36 of [[extractions.md]][^of 11 files listed in step 36 (ie inc 1 file added as per step 46), 9 have no content and 2 have content so this section extracts content only for these latter 2 files.]

in [[vertices.csv]]

```
gid,vertex,vocab,type
vaa0000,vertices.csv,ioa,0000445
vaa0001,vertices.csv-metadata.json,ioa,0000445
vaa0002,edges.csv,ioa,0000445
vaa0003,edges.csv-metadata.json,ioa,0000445
vaa0004,d-function.csv,null,null
vaa0005,d-function.csv-metadata.json,ioa,0000445
vaa0006,authorities.csv,null,null
vaa0007,authorities.csv-metadata.json,ioa,0000445
vaa0008,works.csv,ioa,0000445
vaa0009,works.csv-metadata.json,ioa,0000445
vaa0010,graph.csv-metadata.json,ioa,0000445
vaa0011,null,ioa,0000445
```

in [[vertices.csv-metadata.json]]

```
{
"@context": ["http://www.w3.org/ns/csvw", {"@language": "en", "@base": "http://example.org/"}],
"@id": "vaa0000",
"@type": "Table",
"url": "vertices.csv",
"tableDirection": "ltr",
"tableSchema": {
                "@type": "Schema",
                "primaryKey": "gid",
                "columns": [
                            { 
                            "@type": "Column",
                            "name": "gid",
                            "virtual": false,
                            "required": true,
                            "datatype": null,
                            },
                            { 
                            "@type": "Column",
                            "name": "vertex",
                            "virtual": false,
                            "required": false,
                            "datatype": null,
                            },
                            { 
                            "@type": "Column",
                            "name": "vocab",
                            "virtual": false,
                            "required": false,
                            "datatype": null,
                            },
                            { 
                            "@type": "Column",
                            "name": "type",
                            "virtual": false,
                            "required": false, 
                            "datatype": null,
                            "propertyURL": null,
                            }
                            ]
                }
}
```

## observations

this section contains free-form notes of observations during steps 45-50 of [[extractions.md]]

1. vertices listed in [[vertices.csv]] aren't properly vertices of the graph but we need to specify what we mean by this,
2. the graph's *proper* vertices should be as follows,
    - authorities ie persons,
    - works ie creations inc extracts,
    - events ie temporal-things inc statistics ie measurements,
    - geographic things ie shapes,
    - nothing else,
3. the grpah's *proper* edges should be binary relations as follows,
    - from edge e_i to e_i ie a loop,
    - from edge e_i to e_j where e_i and e_j are not identical ie a non-loop,
    - nothing else,
4. given the above we may want to use BFO to formalise the above,[^note [latest OWL implementation of BFO](https://github.com/BFO-ontology/BFO) has 35 owl:Classes ie OWL implementation specifies classes only and does not specify relations (further per Guide sec 0 *BFO 2.0 OWL is a classes-only specification. The incorporation of core relations has been held over for a later version.*)]
    - begin formalisation,
    - let graph be as follows,[^as per footnote 6 of [[algorithmic.md]] ie the structure we are meant to have is a graph (variously called a quiver ie directed pseudograph ie directed graph ie digraph ie directed multigraph eg [per wolfram](https://mathworld.wolfram.com/Pseudograph.html) and eg [per ncatlab](https://ncatlab.org/nlab/show/pseudograph)).]
        - begin output,
        - take the usual mathematical primitives eg points, sets.
        - let naturals N = {0,1,2,...},
        - let a binary relation ~ on set A and set B be set R = ~ a subset of A * B ie of the cartesian product of A and B where we allow A = B,
        - let a partial unary function f from A to B ie a unary function f from A to B be a binary relation ~ on A and B where for any a in A if a ~ b_i and a ~ b_j then b_i = b_j ie if f(a) = b_i and f(a) = b_j then b_i = b_j,
        - let a total unary function f from A to B be a unary function g from A to B where for any a in A there is at least one b in B such that f(a) = g(a) = b,
        - let vertices V = {0,1,2,...,n) for natural n > 0, 
        - let edges E = {0,1,2,...,m) for natural m > 0,
        - let total unary function d: E to P(V * V) for power set P(V * V) of V * V take each edge e to the subset of V * V of exactly those vertices (v_i,v_j) where e starts at v_i and ends at v_j (again, allowing v_i = v_j),
        - let graph G = (V,E,d),
        - end output,
    - further require that each vertex v_0,...,v_{n-1} in V represent ie stand-in-for,
        - begin output,
        - all v_i are an [entity](http://purl.obolibrary.org/obo/BFO_0000001) per [Guide sec 2.1](https://github.com/bfo-ontology/BFO/wiki),
        - any v_i is exactly one of [occurrent](http://purl.obolibrary.org/obo/BFO_0000003) or [continuant](http://purl.obolibrary.org/obo/BFO_0000002) per Guide sec 2.13,
        - if v_i is a continuant, it is exactly one of [s-region](http://purl.obolibrary.org/obo/BFO_0000006) (eg spatial or geospacial points, lines, shapes)
        - `further-detour-at-13.43` taken,
        - end output,
    - `further-detour-at-13.43` taken to skim the [BFO Guide](https://github.com/BFO-ontology/BFO) so as to specify the formalisation started above within sec **observations** of this file,
        - begin output,
        - BFO tree in Guide fig 1 in page 3,
        - all BFO terms are universals ie types per Guide sec 1.1 in page 3 (further Guide sec 2.1 says "see [19, 25]" re BFO usage of *instance* and *universal*),
        - BFO relations given in Guide sec 2.2 in page 7 ie binary relations as instance-instance, universal-universal, and instance-universal (ie no universal-isntance relations),
        - BFO relations are not within entity per Guide sec 2.2 (probably though this is uncertain as of 13.58 given caveat in same section),
        - *instance* used in BFO as synonym for particular ie entities located in specific regions of space and time per Guide sec 2.6,
        - relations defined for any entity in Guide sec 2.12 are instance_of for particular-universal, is_a for universal-universal, exists_at for particular-particular,
        - end output,
    - null,
    - end formalisation,
5. abort step 4,
6. we restart formalisation in step 4 as follows,
    - begin formalisation,
    - let graph G = (V,E,d) as in step 4,
    - we now want to define j > 0 total unary functions f_0,...,f_{j-1} from V to set {0,1} to further formalise V,
    - let f_0 be a total unary function from V to {0,1} where f_0(v_i) = 1 if v_i *is a universal*, f_0(v_i) = 0 else, where v_i *is a universal* iff `null`,[^eg represented by upper-case variables in Guide per Guide sec 1 page 2 further eg named by italicised nouns in Guide per Guide sec 2.1 page 6.]
    - ~~let `class` be a total unary function from V to {0,1} where `class(v_i) = 0` if `v_i = v_i`, else `class(v_i) = 1`,[^ie for any v_i we stipulate v_i is_of BFO_OWL_CLASS for at least one BFO_OWL_CLASS where is_an_instance_of = BFO relation **instance_of** and BFO_OWL_CLASS = one of 35 owl:Classes in the OWL implementation of BFO.]~~
    - end formalisation,
7. abort step 6,
8. `further-detour-at-15.38` to get markdown syntax for mathematics,
9. we restart formalisation in step 4 as follows,
    - begin formalisation,
    - say \\( A \\), \\( B\\) are arbitrary sets,
    - say \\(A\times B \\) is the cartesian product of \\( A \\) and \\( B\\),
    - say \\( \wp(A) \\) is the powerset of \\( A \\),
    - define a *binary relation* \\( \sim \\) from \\( A \\) to \\( B\\) (ie over \\( A \\) and \\( B\\)) as \\( \sim\;\subseteq A\times B\\),
    - define a *partial unary function* \\( f\colon A\to B \\) as \\( f = \;\sim \\) for *binary relation* \\( \sim \\) from \\( A \\) to \\( B\\) where we have if \\( a_i\sim b_i \\) and \\( a_i\sim b_j \\) then \\( b_i = b_j \\) (ie if \\( f(a_i) = b_i\\) and \\( f(a_i) = b_j \\) then \\( b_i = b_j \\)) for each \\(a_i \\) in \\(A\\) and zero or more \\(b_i\\), \\(b_j\\) in \\(B\\),
    - define a *total unary function* \\( g\colon A\to B \\) as \\( g = f \\) for *partial unary function* \\( f\colon A\to B \\) where we have \\( f(a_i)=b_i\\) (ie \\( g(a_i)=b_i\\)) for each \\(a_i \\) in \\(A\\) and at least one \\(b_i\\) in \\(B\\),
    - now let \\( V=\{v_0,\ldots,v_{n-1}\} \\) for \\( n>0 \\),
    - and let \\( E=\{e_0,\ldots,e_{m-1}\} \\) for \\( m>0 \\),
    - and let \\( d\colon E\to \wp(V\times V) \\) for *total unary function* \\(d\\),
    - and finally let \\[ G=(V,E,d) \\]
    - call \\(G\\) a *graph*,
    - end formalisation,
10. we call the formalisation in step 9 as being up to *graph*,
11. we continue formalisation started in step 9 as follows,
    - start formalisation,
    - say \\( O_v \\) is our chosen ontology or vocabulary for \\(v_i\\) in \\(V\\) where \\( O_v=\bigcup_{i=0}^{i=j-1} O_{v_i}\\) for \\(j>0\\) and where \\(O_{v_0}\\) is the set of the 35 classes specified in [BFO 2.0 OWL](https://github.com/BFO-ontology/BFO),[^and stipulate no \\(o_{v_j} \\) in \\( O_v\\) is a *particular* where we do not define *particular* but elucidate it as *a particular is a spatiotemporal instance ie not a universal nor type eg extended things eg concrete things counter-eg abstract things*]
    - define *complement* \\(\not\sim\\) from \\(A\\) to \\(B\\) (ie over \\(A\\) to \\(B\\)) as \\( \not\sim\;\subseteq A\times B\\) where \\( a_i\not\sim b_i \\) iff not \\( a_i\sim b_i \\),
    - consider *binary relations* \\(\sim_{v_i}\\) over \\(V\\),[^ie from \\(V\\) to \\(V\\).]
    - let \\(v_i\sim_{v_0}v_j\\) iff \\(v_i\\) is a *particular* and \\(v_j\\) is a *particular*,[^where we do not define *particular* but elucidate it as *a particular is a spatiotemporal instance ie not a universal nor type eg extended things eg concrete things counter-eg abstract things eg things in actual spacetime*]
    - then \\( \sim_{v_0}\subseteq V\times V\\) is not empty,[^ie at least some of our vertices are *particulars* eg all those to-be-extracted from files in subsec events of [[tagged.md]] seem like *particulars* rather than not]
    - further \\( \not\sim_{v_0}\subseteq V\times V\\) is not empty,[^ie at least some of our vertices are not *particulars* eg all those to-be-extracted from files in sec topical groupings of [[tagged.md]] (other than files in subsection events) seem unlike *particulars* rather than like]
    - consider *binary relations* \\(\sim_{{vo}_i}\\) from \\(V\\) to \\(O_v \\),
    - let \\(v_i\sim_{{vo}_0}o_{v_j}\\) iff \\(v_i\\) is a *particular* and \\( v_i\; \mathrm{instance\_of}\; o_{v_j}\\) for \\( \mathrm{instance\_of}\; =\;\\) **instance_of** relation specified in BFO 2.0 non-OWL,[^recall no \\(o_{v_j} \\) in \\( O_v\\) is a *particular*] [^where BFO 2.0 non-OWL is either the natural-language or logical-language specification of BFO 2.0 but not the OWL specification.]
    - and let \\(v_i\sim_{{vo}_1}o_{v_j}\\) iff \\(v_i\\) is not a *particular* and \\( v_i\; \mathrm{is\_a}\; o_{v_j}\\) for \\( \mathrm{is\_a}\; =\;\\) *is_a* relation specified in BFO 2.0 non-OWL,
    - and let \\(v_i\sim_{{vo}_2}o_{v_j}\\) iff \\(v_i\sim_{{vo}_0}o_{v_j}\\) or \\(v_i\sim_{{vo}_1}o_{v_j}\\), 
    - then \\( \sim_{{vo}_2}\subseteq V\times O_v\\) is not empty,[^ie each vertex is an instance of or a subtype of at least one class ie term in our chosen ontology ie vocabulary]
    - further \\( \not\sim_{{vo}_2}\subseteq V\times O_v\\) is empty ie \\( \not\sim_{{vo}_2} = \emptyset\\),
    - further 
    - end formalisation,
12. `further-detour-at-19.21` taken to further elucidate *particulars* in step 11 above,
    - begin output,
    - ~~say *this* extended universe ie *this* actual spacetime may be satisfactorilly modelled ie represented by at least one structure within \\(n\\)-dimensional space,[^eg ][^ with concepts used here (eg *satisfactorily model*, *structure within \\(n\\)-dimensional space*) not defined but naively elucidated as usual eg in logic eg in maths]~~
    - skim [Guide sec 4 no 19](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3104413/),
        - begin output,
        - per sec 1.3, ontologists, when building ontologies, should  conceive the world as including entities of two sorts – called ‘particulars’ (or ‘instances’) and ‘types’ (or ‘universals’), respectively, where ‘particulars’ are the sorts of things that can be described on the basis of observations performed eg in the lab or clinic ie are concrete individual entities (entities that exist in space and time and that exist only once), while ‘types’ are to be understood as counterparts in reality of (some of) the general terms used in the formulation of scientific theories ie are to be understood as *repeatable*,
        - per sec 1.3, for each given type, we can in principle discover of indefinitely many particulars that they are its instances,
        - per sec 1.4, *not* all sets ie classes ie pluralities of particulars represent or correspond to a type (eg the pluralities referred to by *particulars which have been measured*, *particulars which are either a fly or a music box*, *particulars belonging to the King of Spain*, etc, do not represent any types while eg *particulars which are electrons* represent at least one type namely type *electrons*), though should nonetheless assume all terms in an ontology *do* refer to types,
        - end output,
    - skim [Guide sec 4 no 25](http://ceur-ws.org/Vol-222/),
        - begin output,
        - per page 58 left column, we start out from a distinction of three levels of entities which have a role to play wherever ontologies are used: Level 1: the objects, processes, qualities, states, etc. in reality (for example on the side of the patient); Level 2: cognitive representations of this reality on the part of researchers and others; Level 3: concretizations of these cognitive representations in (for example textual or graphical) representational artifacts.
        - end output,
    - now attempt elucidation of *particular* as follows
        - begin output,
        - distinguish logical ie abstract space or spaces (inc mathemathical),
        - abort this attempt at 20.40,
        - end output,
    - end output,
13. pause at 20.40,
14. continue at 23.43,
15. `further-detour-at-23.43` taken to see whether specification may be helped by strict or loose model-theoretic language or concepts,
    - being output,
    - as per [Shani Notes](https://people.math.harvard.edu/~shani/Teaching/141/141A-Notes.pdf) or [nCat](https://ncatlab.org/nlab/show/model+theory),
    - ~~define language \\(L=L_s\cup L_l\\) for \\(L_s\\) with non-logical symbols of the language and \\( L_l\\) with logical symbols of the language,~~
    - ~~say \\(L_s\\) has only symbols \\(\sim_0,\ldots,\sim_{j-1}\\) for some arbitrary \\( j>0\\),~~
    - ~~and say \\(L_l\\) has only symbols \\(x_0,\ldots\\) for variables, \\(=\\) for identity, \\( \mathrm{for\ all}\;\\) and \\( \mathrm{for\ some}\;\\) for quantifiers, \\( \mathrm{if\ all}\;\\)~~
    - or rather, set symbols \\(L= L_0\cup L_1 \\) where \\(L_0\\) has the 144,697 characters in [Unicode 14.0.0](https://www.unicode.org/versions/Unicode14.0.0/) while \\(L_1 = \{\sim_0,\ldots,\sim_{n-1},x_0,\ldots,x_{m-1} \}\\) for \\( n,m>0\\),
    - and further define sentences as usual (ie via terms, atoms, formulas),
    - and further define structure \\(\mathcal A = (A,\sim_0^{\mathcal A},\ldots,\sim_{n-1}^{\mathcal A}) \\) with \\(A\\) as domain (eg \\(\mathbb N\\)) and each \\( \sim_i^{\mathcal A}\\) an interpretation of \\(\sim_i\\) in \\(A\\),
    - end output,
16. pause taken on 23 aug 2022 1.16,
17. null