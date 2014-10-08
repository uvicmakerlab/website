# From Grain to Glitch: Simulating Microsound
Patrick Close on September 8, 2014   Makerspace  - 

<p>Since January, I have been researching the history of microsound, which begins, by no means tepidly, with the claim that all sound can be represented as an assemblage of elementary sound particles. Today, microsound refers to both an approach to sound synthesis and a subset of electronic music that operates at this microscopic level of the sound particle, rather than the sound wave.</p>
<p>What is a sound particle? Technically, it is any sound with a duration between 1 and 100 milliseconds; but more precisely, the sound particle was an answer to Iannis Xenakis&#8217;s question, <span class="pullquote">“What are the possible restrictive limits of human psychophysiology?”</span> (<a title="learn more" href="http://books.google.ca/books?id=y6lL3I0vmMwC&amp;source=gbs_navlinks_s" target="_blank"><em>Formalized Music </em></a>45, 47). Xenakis was the founder of microsound. In a series of articles written between 1960 and 1961, he outlined his vision of stochastic music and demonstrated how sound may be represented as a cloud of sound particles within a three-dimensional vector space that could be controlled statistically; by doing so, Xenakis argued, one could synthesize any instrumental or natural sound event and, most importantly, create new, evermore complex sonic entities. This granular approach renders sound scalable and unified, permitting a continuous movement from the ephemeral click to the stochastic mass to the pure sine tone and finally to white noise (and back again). Xenakis proposed the sound particle as a speculative abstraction intended to place sound on a basis independent from musical tradition and habit and to promote a materialist representation of human perception, wherein the whole gamut of human hearing was taken as the point of departure and the destination for music composition and sound synthesis. At least, that&#8217;s how it all began.</p>
<p>Around the mid-1990s, with the proliferation of personal computers and digital audio workstations, microsound drifted from this bedrock premise and instead found itself preoccupied with the possible restrictive limits of digital signal processing. Here, rather than the sound grain on the threshold of human hearing, we confront the glitch or error usually flushed down the drain pipes of digital media. In fact, in the early 21st century, microsound more or less resolved into a genre anchored in simulating digital failure&#8212;microscopic glitches, clicks, and pops, otherwise produced by systemic failure and hardware error, are simulated by means of granular synthesis. Notably, in the discourse surrounding microsound, these near-imperceptible sounds are abstracted into an evocative materiality&#8212;namely, as microscopic matter that intrudes destructively into digital systems; a varied mixture of microscopic material conceits abound, such as “drops, specks, molecules, cells, electrons, dust motes” and other &#8220;digital detritus&#8221; (<a title="learn more" href="http://www.tandfonline.com/doi/abs/10.1080/0749446032000156937#.VA3YWGRdUc8" target="_blank">Whitelaw</a> 95). Consequently, the sound particle fuses with digital noise and error to become recalcitrant indeterminate matter, lurking beneath the &#8220;normal&#8221; operation of computer systems. In turn, microsound artists are themselves characterized as heretical rag-pickers, delving into the navigable subterranean depths of the digital realm, discovering and salvaging the unforeseen, new, and otherwise imperceptible objects called glitches. While microsound inherits its glitch aesthetics from the circuit-bending practices, its glitches, pops, and clicks are generated far away from circuit boards, alligator clips, and soldering guns. Microsound artists simulate failure. For this reason, <span class="pullquote">microsound traffics in what has been called &#8220;glitchalike&#8221;</span> rather than &#8220;glitch,&#8221; <em>per se</em>.</p>
<p>These two broad dispositions&#8212;one starting in the 1950s, the other around 1996&#8212;demarcate two beginnings of microsound, a divide I’ve come to represent as one between the grain and the glitch, both of which lay claim to the sound particle but present it in radically different ways. To be clear, the shift of the above limit-question&#8212;from grain to glitch&#8212;is not a difference in scope (i.e., from human audition to something like computer audition), but rather a difference in kind: Xenakis’s materialist, humanist epistemology and program collapses into an informatic ontology. The original abstraction of the sound particle adequate to a materialist conception of human perception capitulates to the reification and fetishization of indeterminancy, fused with a lyrical obsession with &#8220;materiality.&#8221; To wit, <span class="pullquote">the glitch of microsound is deliberate, not accidental; it is designed, not discovered</span>. In this way, the digital aesthetic it propounds hinges on precisely what it is not. Construing pure chance as a radical ontological element, as liberatory, rather than just a function of ignorance, was anathema to Xenakis and, in fact, provided a foil to his project of microsound, which he understood as the rationalization of chance through the use of probability theory.</p>
<p>While most of my research is devoted to drawing out Xenakis’s legacy (centred around his works and writings from 1954 to the late 1970s), its vanishing point is nevertheless that nebulous fulcrum, 1996. My first question was to ask how these two approaches within microsound were related&#8212;whether merely nominally or methodologically or otherwise&#8212;and moreover I had to ask the more basic question of <span class="pullquote"><em>how to make a sound particle</em></span>. I aimed to build a model that could move from grain to glitch in a minimum amount of steps, while also being of pedagogical value (to myself and others) in terms of elucidating both concepts. I wanted to program a synthesizer that was not just another whiz-bang device or inelegant mess. My process involved scouring community forums, extracting bits and pieces of others&#8217; code, and cobbling together a model that was both compact and faithful to the basic outlines of Xenakis’s original conception of microsound and granular synthesis detailed in his book, <em>Formalized Music</em>.</p>
<p><a href="http://maker.uvic.ca/wp-content/uploads/2014/09/grainglitch.png"><img class="alignnone size-full wp-image-4597" src="http://maker.uvic.ca/wp-content/uploads/2014/09/grainglitch.png" alt="Max Patch by Patrick Close" width="1150" height="720" /></a></p>
<p>To create this model, I turned to Max/MSP, a real-time visual programming language and one of the critical programs released around 1996 that contributed to the sea-change in microsound, planting the sound particle within the soil of real-time digital signal processing and placing it in the hands of artists outside institutional walls. Max/MSP is centred around the idea of a &#8220;patch,&#8221; borrowed from the history of analog modular synthesizers, in which a sequence of objects&#8212;processes or programs&#8212;are patched together with chords, creating a single system. Now, for many years, the basic materials of microsound comprised of orchestral ensembles, probability distributions, analog oscillators, magnetic tape, splicers, punchcards, and batch-processing mainframe computers. So, of course, there exists a rather severe anachronism in using real-time signal processing programs to represent labour-intensive and non-real time processes; in this case, however, I was primarily interested in the formal relations between the grain and the glitch. Nevertheless, the drastic interface shift from the punchcard to real-time processing cannot be forgotten but nor should the shift from mediation-as-process to mediation-as-world, as I believe we see between the grain and the glitch, be forgiven as just a matter of technological change.</p>
<p>In any case, <span class="pullquote">the anachronism of simulation proved productive</span>, allowing me to renegotiate Xenakis through the obscured lens of his estranged successors. I would argue that Xenakis, too, had an aesthetics of failure. His interest in stochastic clouds of sound derives from his experience in fighting in the National Liberation Front of Greece. As a Communist and youth leader, Xenakis organized and participated in many mass demonstrations, many of which ended in clashes with Italian and German fascists but also British imperialists. Xenakis claimed microsound was born out of being haunted by “the passage from complete order to total disorder in a continuous or explosive manner” (<em><a title="learn more" href="http://books.google.ca/books?id=y6lL3I0vmMwC&amp;dq=%22the+passage+from+complete+order+to+total+disorder+in+a+continuous+or+explosive+manner%22&amp;source=gbs_navlinks_s" target="_blank">Formalized Music</a> </em>9) that he experienced in such mass demonstrations and clashes. All else being equal, that strikes me as a good working definition of glitch. The difference lies between how Xenakis saw an epistemic challenge&#8212;to grasp complex swarms as rule-governed entities&#8212;and contemporary microsound sees the radical shock of the anomalous, full stop. (It&#8217;s worth noting that Xenakis was reading Plato and Lenin while involved in the Greek resistance, and contemporary microsound artists traffic heavily in post-1968 theory and &#8220;accelerationists,&#8221; including Deleuze, Lyotard, and Baudrillard.)</p>
<p>In the interest of saving my model from spinning in a void, emulation became an increasingly crucial factor in simulating microsound. I searched personal directories to find any granular synthesis software from the mid-1990s. My original assumption was that real-time programs enforced the representation of the sound particle as an ontological entity rather than a set of rules and procedures; that is, until I encountered Th0nk (released in 1995), which is a non-real time granular synthesizer. Rather than traversing a field of evolving sound, the user inputs a sound file , which is then processed and outputted for later listening. Yet, Th0nk&#8217;s rhetoric feels both prescient and parodic with regard to the rhetoric of later microsound: the manual promises the thrill of &#8220;NO CONTROL WHATSOEVER&#8221; and the ability to &#8220;to harvest fresh, unanticipated material . . . without having to think at all.&#8221; Here, as an end-user, the microsound artist enters the marketplace of &#8220;digital detritus.&#8221;</p>
<p><a href="http://maker.uvic.ca/wp-content/uploads/2014/09/th0nk.png"><img class="alignnone size-full wp-image-4598" src="http://maker.uvic.ca/wp-content/uploads/2014/09/th0nk.png" alt="th0nk" width="1150" height="838" /></a></p>
<p>It&#8217;s at this juncture that we encounter&#8212;to put it strongly&#8212;a rupture in microsound&#8217;s history, wherein Xenakis&#8217;s original materialist program is inverted into a &#8220;radical&#8221; (or regressive) ontology. But how can simulation provide an argument about what persists and what changes across two ostensibly different aesthetics? And to what extent can such a model afford critical speculation about extended notions of the sound particle, failure, and microsound, considered in a more unified way?</p>
<p>Accordingly, my aim was conservative in essence: I wanted to see whether the present was beholden to the past, whether Xenakis’s thoroughly materialist approach could be possibly rehabilitated as a corrective to the glitch or so-called digital aesthetics of contemporary microsound. And I had to acknowledge that any straightforward critique of contemporary microsound risks rehearsing the very same gestures of microsound itself: namely, unearthing disruptive contingencies&#8212;the unforeseen &#8220;glitches&#8221; of microsound&#8212;and arranging them in a new form (i.e., an essay or argument). Rather than exposing how contemporary microsound&#8217;s alleged digital aesthetics and politics is shot through with contingencies, I was interested in seeing to what extent it was still constrained by an idea of the sound particle as an abstract rule for musical realization, as proposed by Xenakis. After all, Xenakis&#8217;s method of sound synthesis was itself a cogent theoretical (and political) argument that claims that there is <span class="pullquote">no salvation in pure chance or pure contingency</span>: neither local improvisation nor global genealogies are sufficient, in Xenakis&#8217;s view, to unburden us of tradition and habit or, moreover, to provide us with the resources to grab a hold of whatever burdens us.</p>
<p>By creating a patch in Max/MSP, I ended up sifting the generation of sound particles out of Xenakis’s writing, in three “dimensions”&#8212;pitch, intensity, and duration&#8212;to produce a stream or cloud. As a cloud-like system, one can control the entropy of a sonic entity (like Maxwell’s Demon) as Xenakis envisioned it. A sonic cloud can range from pure periodicity or complete disorder (understood as the “chance” flux of a range of values determined probabilistically). Or, more broadly, it can range from grain to glitch. <span class="pullquote">Like all models, mine was reductive&#8212;and I hope in the most productive sense.</span> And while I had initially approached simulation as an abstract exercise in order to grasp certain concepts I did not quite understand, at every turn, simulation was confronted by emulation, abstraction by material practices, and real-time processes by non-real-time processes. In aiming to simulate or (re)enact a number of Xenakis&#8217;s key arguments, simulation offered the opportunity to transcode between these different registers.</p>
<p>Below&#8217;s the code for my Max patch, if you want to give it a try.</p>
<style type="text/css">
  .gist {width:1150px !important;}
  .gist-file
  .gist-data {max-height: 500px;max-width: 1150px;}
</style>
<p><script src="https://gist.github.com/jentery/7b876a37d9ea600d1009.js"></script></p>
<p>Post by <a title="learn more" href="http://maker.uvic.ca/author/patrick">Patrick Close</a>, attached to the <a title="learn more" href="http://maker.uvic.ca/category/makerspace/">Makerspace</a> category, with the <a title="learn more" href="http://maker.uvic.ca/tag/physcomp/">physcomp</a> tag. Images for this post care of Patrick Close and Th0nk.</p>