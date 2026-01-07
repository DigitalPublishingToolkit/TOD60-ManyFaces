---
Pr-id: MoneyLab
P-id: INC Reader
A-id: 10
Type: article
Book-type: anthology
Anthology item: article
Item-id: unique no.
Article-title: title of the article
Article-status: accepted
Author: name(s) of author(s)
Author-email:   corresponding address
Author-bio:  about the author
Abstract:   short description of the article (100 words)
Keywords:   50 keywords for search and indexing
Rights: CC BY-NC 4.0
...


**A Subject Access Request, Then What?**

> (Un)structuring Online Analytics for Data Institutions

*Jake Stein and Reuben Binns*

Collecting, storing, analysing, and distributing information derived
from disparate data sources have become radically easier in the past
decade. The proliferation of big data analytics and algorithmic
technologies is thanks to advances at every stage in the data analytics
pipeline from ingestion to visualization, and at each layer of the data
analytics stack from hardware to user interface.^1^ Organizations with
access to sufficient capital have access to tools which quickly and
reliably convert upfront investment into valuable insights and system
optimizations. Indeed, a vast and growing set of systems have themselves
been progressively optimized to the needs of large organizations –
resulting in generalizable workflows and plugand-play architectures for
turning big data into material gains for enterprises with access to
valuable troves of data.^2^

At the same time, it has become increasingly apparent that resisting the
(mis) use of big data and algorithmic technologies requires the use of
sophisticated data analytics too. Advocates seeking transparency,
privacy, or agency with respect to these systems often analyse the very
same data that platform corporations rely on for their own
operations.^3^ For efforts that resist platform information asymmetries
through collecting and analysing data in pursuit of algorithmic
transparency or regulatory action, achieving sufficient scale is not
straightforward. The cost of technologies and contracted expertise
necessary far exceed grassroots budgets. Big data analytics software has
been developed with the needs of centralized, hierarchical structures of
corporate practitioners in mind and is poorly suited to the distributed
governance and open access to which activists and academics aspire.
Despite new technologies’ potential to be used in challenging
information asymmetries, novel analytics technologies demand enormous
upfront investment and sustained overhead cost. Big data is only
valuable when it scales, and big is expensive.

One approach to mitigating the inherent gulf of resources between
platforms and advocates who seek transparency and agency within
corporate systems is to pool resources or form coalitions across civil
society and academia under novel data governance models – what the Open
Data Institute (ODI) has called ‘Data Institutions’.^4^ The ODI defines
these broadly as ‘organizations whose purpose involves stewarding data
on behalf of others, often towards public, educational or charitable
aims’.^5^ Similarly, participatory action research (PAR) has allowed
academia to become an important host for infrastructures supporting
adversarial data aggregation, working with advocates to audit
algorithmic systems or create tools capable of computationally mediating
solidarity against overreaching algorithmic control.^6^ These functions
align closely with the ODI’s specification of ‘Bottom-up Data
Institutions’, referring to organizations containing ‘processes that
enable people – usually those that have generated the data or that the
data is about – to actively take part in those data governance
processes’.^7^

However, the academy faces a platformization crisis of its own, with
universities increasingly supplanted as centres of computational power
by cloud-computing providers that offer cheap flexible compute, while
academic research budgets are meagre compared to those of corporations
and university administrations closely guard valuable intellectual
property.^8^ While of course the flexibility of cloud computing can also
accelerate computation-heavy research, the institutional power granted
by a standing reserve of computational power is a card now held closely
by industry.^9^ Furthermore, access to enormous datasets generated on
platforms leaves academic research at a disadvantage in data access.
Data subjects, activists acting in their behalf, and academics all find
themselves in similarly undesirable positions vis-à-vis platform
hegemons, but also possess complementary resources for developing
alternatives to serve the public interest.

Regulators have begun to recognize and address information asymmetries,
but provide only meagre tools for data subjects or data institutions to
combat asymmetries in practice. In many jurisdictions, data access
rights face headwinds as they wrongfully pit data subject rights as
restraints against governments’ efforts to energize the development of
artificial intellience (AI) and boost their constituent economies.^10^
Individual data access regimes contained in data protection regulations
like the General Data Protection Regulation (GDPR), 2018, and the
California Consumer Privacy Act (CCPA), 2018, and aggregate data access
rights for researchers contained in successive regulation like the
Digital

A Subject Access Request, Then What? 201

Services Act (DSA), 2024, as well as voluntary access to research
application programming interfaces (APIs) provide a convenient side
door, allowing activists and researchers to access data without facing
the costs of constructing net-new data collection infrastructure
themselves. Indeed, scholarship and litigation both have made
significant progress in asserting the collective use of subject access
rights for this purpose.^11^ Data collection (or access) is, however,
only the first step. Information asymmetries can only be counteracted
when subjects have access to *information* contained in their data too,
requiring suitable data analytics systems to complement their
access.^12^ Financing, creating, and governing these systems require
navigating the incentives, constraints, and priorities of all of the
parties involved, ranging from data subjects themselves to civil society
funders, advocacy organizations, and academic researchers.

We examine the politics of this coordination as we navigate the
challenges of co-constructing data pipelines alongside activists from
Worker Info Exchange (WIE) which seek to use data subject access
requests (DSARs) to afford workers transparency and agency within
algorithmic management by platform work apps.^13^ In particular, we
address the obstacles that arise while contending with the structure
that DSAR data contains in order to draw attention to the conflicting
epistemologies layered in the schemas, ontologies, and metric
definitions involved in its analysis.

Our collaboration with WIE exemplifies the broad variety of stakeholders
necessary for building data institutions capable of counteracting
platform control. Our engagement with WIE is partly supported by the
‘Ethical Web and Data Infrastructure in the Age of AI’ project – a
research programme funded by the Oxford Martin School to design new web
protocols and data architectures which can better promote data subject
autonomy in the platform-dominated web.^14^ We benefit from the
collaboration as a rich case study in which to prototype and test our
designs.

WIE is a non-profit organization closely aligned with the App Drivers
and Couriers Union (ADCU), who represent platform workers in the United
Kingdom (UK) and the European Union (EU). Accordingly, WIE is interested
generally in providing drivers with better information about how to
manage their own activities and income, often by helping drivers seek
evidence to contest mistreatment mediated via algorithmic systems. WIE’s
association with the ADCU means it is also active in collective
advocacy. In a landmark finding, one of WIE’s suits with the ADCU
established the precedent that DSARs can be used for the purpose of
sourcing aggregate data in favour of collective advocacy in addition to
privacy.^15^ At the time of our collaboration, the law firm AWO was
engaged with WIE in investigating algorithmic pricing and work
assignment for platform workers. AWO is a UK ‘law firm and consultancy
that empowers individuals and organizations to uphold data rights,
comply with the law and effect change in data protection and digital
policy’.^16^ Finally, the most critical stakeholders are the data
subjects themselves – workers who use gig economy apps. Workers
participate in this institution by requesting access to their data via
WIE. WIE then processes the request with Uber on the driver’s behalf, in
exchange pooling that data in aggregate form. Driver data is held by WIE
and has been shared with us for the purpose of conducting research and
providing insights.^17^ Workers stand to gain both in terms of greater
transparency into their own data and from the results of collective
advocacy that aggregate analyses of their data supports.

Taking the design decisions that we observed and made ourselves when
building data structures as the site of our research, we illustrate the
impacts of data structure on the meaningful access to information
contained in it. With the hope of setting out a blueprint for future
architectures for data institutions, we evaluate how various data
structures serve or privilege individual perspectives within the tangle
of incentives existing among the collaborating parties and stakeholders
mentioned.

In the design of multi-stakeholder public-service data architectures, we
emphasize the need to consider that the same underlying data might
simultaneously serve numerous purposes or communicate divergent
interpretations depending on its structure (how data is categorized in
fields, organized into tables, and aggregated into metrics). By
‘infrastructure’, we mean the technical systems, databases, and
organizational processes through which this data flows.^18^

To capture the polysemous quality of data, we borrow Slavoj Žižek’s term
‘parallax view’ to analogize how data staged in a unified underlying
architecture can support many (even conflicting) pursuits and
epistemologies.^19^ Put simply, a parallax effect occurs when two
observations of the same event differ due to perspective. By borrowing
the concept of the parallax, we explain that despite having access to
the same underlying data (the *observed* *event*), the structure in
which that data is provided (the *perspective*) can radically alter the
information accessible within it. Žižek uses this phenomenon as an
allegory for his system of reason, while here we use the term to
describe the relationship between data and its structure, which is
relevant to our pursuit in several ways. First, at the lowest level, it
helps illustrate the contingency of data’s meaning upon its context and
which other data or knowledge it is enriched with. Second, the parallax
could be regarded as an essential quality for data structures meant to
serve different,

A Subject Access Request, Then What? 203

even conflicting end goals – in our case, the empowerment of the
individual to use their data to act more effectively *within* a system,
but also for the collective critique of that system with the goal of
changing its rules and configuration to benefit the data subject. We see
this as a divergence from the typical design goal of analytics systems
geared toward establishing a unified interpretation of data. The
economic and socio-technical demands of large-scale data analytics
systems are in turn co-constructed and co-used by academics, advocates,
and ultimately data subjects. Accordingly, supporting several
contradicting uses or interpretations of data cannot be avoided, even if
the overall end goal is the same. We conclude by suggesting which
technical implementations can simultaneously support conflicting
interests and epistemologies that different parties bring to the data,
without engineering a single perspective into the data’s structure.

# The Implications of Data Structure on Meaningful Data Access

Though any data pipeline may contain a similar mix of technologies,
their configuration depends on the volume, velocity, sensitivity, and
target uses of data.^20^ This section aims to illustrate how decisions
about *where* structure is added along the data analytics pipeline and
*what* structure is added (or left out) can obfuscate meaning in the
data we have processed with WIE. Further, by evaluating the ways data is
obscured in the structure returned by Uber, we demonstrate the
importance of avoiding imparting restrictive structures of our own when
designing technical architectures for data institutions.

## Unpacking Obfuscation

The most straightforward ways data structures can impede meaningful
access for subjects is through *obfuscation*. Finn Brunton and Helen Fay
Nissenbaum famously define obfuscation as a tactic for data subjects to
resist surveillance by making data ‘more difficult to act on, and
therefore less valuable . . . adding to the cost, trouble, and
difficulty of doing the looking’.^21^ In the context of analysing DSAR
responses, obfuscation acts in the reverse, with advocates and academics
‘doing the looking’ into the behaviours of algorithmic systems on behalf
of data subjects and platforms making analysis more difficult for them.

Well-documented examples of obfuscation may be as simple as returning
data in non-machine-readable formats like PDFs (Portable Document
Format) or providing too little contextualizing information for data to
be interpreted.^22^ Here we briefly inventory some of the obstacles to
analysing data we encountered in data structures. The motivation of this
analysis is two-fold: First, it demonstrates that access, human or
machine readability, interoperability, and portability are all concepts
that should be defined contingently on the intended use of the data in
question rather than being held to an objective standard or format. This
point hopefully also emphasizes the role data structure plays in
influencing the meaning one can ultimately derive from the very same
data. Second, this analysis warns that even enhanced access requirements
which stipulate API or database availability under progressive
transparency regulations like the DSA still leave data controllers many
tools to obfuscate important meaning in data that they are compelled to
share.

Presumably, unintentional obfuscation abounds in the data that WIE
received via DSAR responses. For example, data exporting mistakes led to
file errors when processing data – such as extra commas included in CSV
(comma-separated values) files, where commas act as cell delimiters,
thus preventing files from being immediately readable, or the
inconsistent use of data fields with the same names.

## Identifying Problem Structures

The structures that impeded our analysis of data occurred at three
levels: the schema (or table), field (or column), and value (or cell)
(Figure 9.1). Our analysis was obstructed by features of the data which
were present in all of the responses and separately by inconsistencies
in the structure within responses themselves or between responses when
aggregated or compared. These structures and inconsistencies among them
can be attributed to any number of origins. We expect some might arise
from Uber’s own internal systems changing over time to support different
features which may require more, less, or different forms of data. They
might, likewise, emerge from differences between formats convenient to
the functional needs of Uber’s systems and the transformations performed
to prepare data request responses. Whether these layers of structure
were intended to obscure elements of data or make the response compliant
with the requirements of DSARs under the GDPR is not discernable. After
all, a DSAR is far from the natural state of data otherwise meant to
function as part of a living, moving operational system.

Further, Uber arguably cannot be expected to foresee all the
calculations that the requester aims to conduct and to process data
accordingly (unless of course they are instructed); nor are data
controllers like Uber expressly obligated to deliver data in its most
disaggregated form. However, we might argue that supplying data in a
disaggregated format is a straightforward and uncontroversial
requirement of interoperability and portability that should require

12/1/22 12/1/22

**Figure 9.1** Schema, field, and data levels of data structure
*Source*: Prepared by the authors.

little marginal effort.^23^ One could even go as far as attributing some
obfuscating data structures provided by Uber as good-faith yet misguided
attempts to provide drivers with the metrics they may more easily
interpret. Intended or not, inconsistencies in data structure had the
effect of obfuscating some of the most contested and controversial
aspects of Uber’s algorithmic management practices and ultimately
demonstrate the need for greater specificity in data standards or access
provisions, while emphasizing the valuable lesson that
counter-architectures should put off structure as long as possible to
facilitate the maximum possible number of further aggregations. With
that in mind, we briefly unpack some of the schema-, field-, and
cell-level obfuscation which held back our analysis.

### The Schema Level

Schema-level structure refers to the decisions made about how many
independent tables a database is composed of, which fields are held in
each of those tables, and the semantic connections (or lack thereof)
that can be made between tables. Data architects meticulously design
schemas in order to reduce the latency of queries when writing or
retrieving data, and to serve the critical purpose of separating data
with varying levels of sensitivity to support table-level access
restrictions. The schema of the tables returned in DSAR responses
provided some immediate clues and artefacts of its designers’
intentions.

On the schema level, two kinds of data structure presented difficulties
in analysing data. First were the differences in the schemas of separate
DSAR responses preventing the software we produced from processing
responses in an interoperable fashion. For instance, some requests
received a file titled ‘Payments’, while other responses updated the
name of that file to read ‘Driver Payments’. Second, and of much greater
consequence, was a lack of semantic structures to connect records of
different types within individual DSAR responses. Most notably, there
was no unique identifier allowing for linkages between payments
(represented independently in ‘Driver Payment’ and ‘Miscellaneous
Payments’ tables) and trips, which were assigned their own table. As
drivers are not paid on a trip-by-trip basis, it is impossible to
sufficiently disentangle the data structure to determine exactly what a
worker was ultimately paid for a specific trip, including all costs,
reimbursements, incentives, and other auxiliary costs. This was further
complicated by the existence of the separate ‘Miscellaneous Payments’
table which provides records of reimbursements or payments for sick
leave, holiday pay, pension contributions, and incentives like rewards
for accepting consecutive trips. This table likewise had no ability to
be linked to individual trip records, even when payments were associated
with the completion of particular incentive or goal.

### The Table Level

A similar link is lacking between the dispatch and trip tables. This
missing link also illustrated how table-level data structures interact
with structures within specific tables. In the dispatch table, rather
than providing individual records of each dispatch offered, accepted, or
rejected, Uber provides hour-by-hour aggregations of dispatches.
Naturally, this aggregation makes links to the trip records (whether or
not they were completed) impossible. Furthermore, it stands directly in
the way of efforts to detect changes in work offered to drivers
depending on their selectivity towards work offered – a behaviour that
drivers anecdotally reported to WIE.

WIE suspects that drivers are implicitly penalized by the algorithmic
systems which assign trips to drivers when they refuse or cancel
unfavourable jobs. Left uncontested, such algorithmically mediated
punishment would afford Uber the ability to maintain their position that
drivers are independent providers free to work as they wish, while still
allowing the platform to influence driver behaviour. In any event, the
ability to independently audit the behaviour of algorithms which are
essential to data subjects should fall within the realm of transparency
expected from data access provisions. This is precisely the grounds
argued for and won by WIE in the Netherlands and continues to be
pursued.^24^ The goal of this article, however, is not to draw
conclusions about which structure should be lawfully provided by data
controllers in DSAR responses. Rather, we aim to highlight the role of
data structure in limiting and enabling different analyses with the goal
of producing designs that facilitate the simultaneous use of the same
data by several parties, thus amortizing the technical infrastructure on
which it relies. The barriers found in data structures provided by Uber
are an excellent example where this is not the case, providing
invaluable lessons for data architecture design.

If individual records of jobs offered, accepted, and rejected by workers
(‘dispatches’ in Uber’s terminology) were accessible, auditing the
existence of algorithmic punishment would be a straightforward
calculation. However, with individual records only provided to drivers
aggregated into hourly totals and with no link (no unique identifier) to
trip records, evaluation of any causal link between cancellations and
work assignment becomes impossible.

To the critical researcher, the decision to aggregate data appears a
frustrating instance of obfuscation, perhaps made to prevent inference
of the logics contained within Uber’s work assignment algorithms. Giving
Uber the benefit of doubt, this aggregation might also be explained as
an intended choice made to facilitate better compliance with GDPR by
providing human readable metrics. The catch-22 of providing more
disaggregated data versus human readable metrics here highlights the
consequences of vague definitions for data portability. However, this is
in many ways a false dichotomy; by simultaneously providing the logic
necessary to aggregate metrics like acceptance rate (or aggregate
metrics themselves) and the most disaggregated data, Uber could satisfy
both needs. The structure of the dispatch records is exemplary of how
data structures become palimpsests of the nested perspectives inscribed
into the final data presented in the response. They overlay the
intentions of the data architect who originally orchestrated the data
collection system to be most effective for Uber’s own purposes, with the
data analyst subsequently tasked with compiling data for a DSAR
response. This layers what Uber is willing to disclose on top of their
interpretation of how to fulfill obligations for access to data
subjects, and of course the artefacts of the source system. Elsewhere in
the DSAR response, records similar to those in the dispatches table are
left disaggregated as is the case of individual trip records.

### The Field and Cell Levels

Finally, data on a cell-by-cell level significantly hampered analysis.
As with schema- and table-level obfuscation, this was the result of both
errors or inconsistencies in data quality and choices made in the design
of the documents. With respect to data quality, we encountered fields in
which the format of data was different even within the same column. For
example, some fields contained timestamps of different machine and human
readable formats, suggesting those resulted from the combination of
other tables. There were also missing values (such as in the vehicle
unique identifier field) in several responses or inconsistent values
between responses, most likely associated with changes to Uber’s own
data formats over time – for example, changes in spelling from ‘en
route’ to ‘enroute’.

Other cell-level structures that obfuscated our analyses were more
indicative of the systems out of which data were sourced. One of WIE’s
primary objectives was to better understand the calculation of fares and
driver pay for individual rides, both to empower drivers with greater
awareness in planning their own activities and to better understand
Uber’s algorithmic ‘dynamic pricing’ scheme. In the ‘Driver Lifetime
Trips’ table, Uber supplied a record for each trip taken by drivers. The
table contains a variety of fields detailing the fare, from ‘Original
Fare’, which Uber’s guidance document clarifies is ‘based on time +
distance’, to ‘Upfront Fare’, which applies to trips with a quoted fare
before acceptance, to ‘Base Fare’, which is defined only as ‘base fare
of the trip’. The table also contains the individual components one
would presumably need to reproduce the end fare paid by passengers, such
as the trip distance, time, and their associated rates, as well as the
surge fare applied to trips. Despite providing these aspects of the
trip, we were unable to consistently reproduce the fares provided; for
instance, in each of the responses we analysed, the formulas for
determining original fare (base fare + distance at distance rate + time
at time rate + surge + service fees) only occasionally lined up with the
fare figures provided elsewhere in the table. Again, these
inconsistencies could equally be attributed to fields being meant for
use in Uber’s system, rather than retrospective analysis, as well as the
actual formula used to generate the fare changing over time. This is
supported by announcements by Uber that they switched from fares
calculated according to rates to a ‘dynamic pricing’ system and that
drivers can access their take-home payments through their app
directly.^25^

## Coping with Obfuscating Structures

The structure of data in Uber’s request responses illustrates how one
can gain access to data without necessarily gaining access to all of the
information contained in that data. We cannot, however, know whether the
intent of the data analysts’ chosen structures was goodwilled clarity of
communicating the driver’s behaviour or obfuscation of the algorithm’s
logic. The effect nonetheless reveals a fundamental tension for the
application of data access policy that goes beyond arguing the
definition of personal data. The importance of data structure results in
situations where a data controller can return personal data from their
systems without returning all of the *information* that data might
contain. In the case of WIE, a Dutch appeals court ruled that more
granular data and specific explanations of algorithmic systems should be
given to drivers, brushing aside claims that this would require
platforms to divulge trade secrets. Such a finding, however, only
emerged from very specific requirements provided upfront by WIE, not on
any independent judgement about data initially returned.

The more granular data and explanations WIE have been able to win are a
step in the direction of a more complete picture of the system. From the
perspective of a system designer, the outcome is, however, bittersweet.
The situation demonstrates that transparency into the decisions of
algorithms or the logic of the systems through which data flows is not
straightforwardly deducible from granular data alone. Further, it is
difficult to expect data consumers to specify the ends they expect to
use data for at the outset, or to know enough about the system’s
underlying structures to specifically request explanations. Indeed, this
suggests that perhaps there is value in preserving the structure
controllers return data in, rather than opting for the most granular
form.

The choice of granular or structured can also be a false dichotomy. With
respect to dispatch data, obfuscation could have been avoided if
aggregation was kept to later stages in the data pipeline and semantic
structures left intact. In any event, in the first instance Uber neither
provides a polished report meant to be understandable to workers nor a
‘raw’ export of the way data exists in their system. Their DSAR
responses are something in-between, demonstrating how the political and
economic interests of parties providing data are inscribed in the data
structure, intended or not.

The obstacles Uber’s DSAR data structures present provide a valuable
example for data institutions that attempt to counteract them. Providing
data available at a lower level of aggregation could help such
infrastructures to avoid repeating this obfuscation while allowing for
greater flexibility in data’s use. A constellation of parties will be
needed to actualize data institutions which aim to provide governance
and transparency to data subjects while also benefitting other
stakeholders like advocates, organizers, and researchers. When data
institutions assume the role of imposing new structures on data for
their own purposes, they will need to be wary about how balancing the
interests of many more parties than merely the platform and data subject
may create similar effects to those we observed here.

DSAR responses are artefacts of the systems out of which they emerge.
This exposes a somewhat expected mismatch between the positivist
imagination of data enshrined in data access regulation and latent (yet
overly optimistic) hope that access to it might be sufficient for
transparency into or means to act against the systems out of which it
flows. It also is a stark reminder of data’s innate subjectivity and
thus the misguided assumption that we can impose one-size-fitsall
‘interoperability’ to data.

Rather than rehash that there is no such thing as raw data or that ‘all
data are local’, we take this analysis as the design prompt for our own
data architectures.^26^ In data institutions functioning as
public-service data architectures or counterarchitectures, should we
strive for data to occupy the role of reflecting the ground truth – an
honest, unadulterated witness to the events it records – or is it more
valuable (or even existentially necessary) that the data still carries
the fingerprints of the developers, analysts, and *systems* through
which it has already passed? The answer, as we see it, depends on
purpose. In the next section, we reflect on the architectures at our
disposal for creating architectures which may support a diverse set of
stakeholder needs without imparting structure which itself obfuscates or
narrows the information available in the data it holds.

# Mapping Data Structures and Their Politics 

Now that we have grappled with some examples of how data structure
restricts and enables the potential information one can extract from
underlying data, we can begin to explore how the interests of the
parties involved in co-constructing data institutions may themselves
manifest in the infrastructures they create. This section proceeds by
exploring how data structure factors into goals of our present work
alongside WIE: to deliver information from DSARs directly to drivers in
a convenient format, to investigate the behaviour of algorithmic pay and
work assignment, and to minimize the workload for WIE to self-manage
their data infrastructure.

We first sought to make workers’ data more accessible and understandable
to them. However, even defining basic metrics for drivers such as
pay-per-hour is inherently political, requiring that we select which
perspective to encode into data structure and present to workers (Figure
9.2). WIE sees hours worked as including time signed on to the app
awaiting new jobs, while Uber discounts this time. As a result,
pay-per-hour-worked looks radically different depending on the logic
used to make the calculations. By way of example, one worker’s data we
examined would have their hourly wage between GBP 23 and GBP 30 per
hour, according to Uber’s formula for the metric, which only includes
time on the way to passengers or with passengers on rides. Accounting
for time waiting, the same driver saw hourly rates hover between GBP 13
and GBP 20 per hour for most of their time working for Uber, with their
gross wage per hour dropping into single digits on occasion. This is, of
course, before costs covered by the driver, including but not limited to
insurance; vehicle maintenance; licence; congestion charges; and fuel.
Indeed, according to their DSAR data, this driver typically spent around
30 per cent of their time online waiting for rides. One important
complication to this metric is the practice of ‘multi-apping’, when
drivers simultaneously use several gig-work apps in hopes of capturing
the best offers and minimizing dead time. This practice is often against
the terms of service for gig-work apps like Uber depending on the
location, but is frequently brought up as a counterargument for paying
for between-ride time.

Returning to the goal of delivering valuable transparency to workers,
generating metrics like the aforementioned wage calculation is best
suited to highly structured, relational data stores akin to those often
used in basic business analytics systems. However, highly structured
data infrastructures only accommodate rigid definitions for metrics to
be repeatedly applied, and as a result they are highly sensitive to even
small changes in underlying data.

Furthermore, encoding rigid definitions (like Uber’s and WIE’s competing
definitions of pay-per-hour) into the structures inherently narrows the
interpretation of the data. DigiPower academy provides an example of
this approach, producing polished and digestible figures for individuals
based on DSAR data.^27^ The advantages of a highly structured
environment lie in the convenience and accessibility of outputs to data
subjects. However, highly structured databases’ sensitivity to changes
in data sources makes them labour- and resource-intensive for
organizers, placing the parties responsible for their maintenance
primarily as intermediaries between platforms and subjects, while
leaving fewer resources to inductively investigate systemic problems.
Furthermore, the risk of entrenching specific narratives or
interpretations into data structures and thus limiting potential
interpretations is a deal-breaker to researchers committed to open
science or advocates like WIE who are interested in uncovering more
systemic patterns within aggregate data without frequently refactoring
their systems.

Our overall design decisions quickly became defined by a core trade-off.
Either we privilege repeatable processes, dedicating time to building
end-user-friendly results backed by a highly structured infrastructure,
or we leave data in a lessstructured form, thus preserving the ability
to conduct deeper iterative analyses. Understanding which route provides
more benefit to the data subject is a fraught exercise of acting within
versus against the greater system. WIE’s investigation of pay and work
assignment algorithms requires an open infrastructure for inductive
analysis and, if successful, could achieve considerable gains in rights
for workers. However, prioritizing the collective interests of data
subjects over individual access to metrics poses a challenge for data
stewardship and their individual agency. Britt S. Paris, Corinne Cath,
and Sarah Myers West have highlighted the penchant for technological
solutions to tack towards value ethics prioritizing efficiency and
perceived good from the top down in place of an approach based in care
ethics which might honour the individual autonomy of data subjects.^28^
Dubal’s ethnographic work, likewise, warns about placing perceived
collective gains ahead of individual agency in gig work.^29^ In our
case, privileging aggregate analysis ahead of individual data access
risks making qualifying all workers as a homogenous set, rather than
empowering them with information directly. On the other hand, though an
algorithmic audit requires diversion of resources from immediate data
analytics outputs directed at data subjects, it could lead to much more
impactful legal victories or proof of algorithmic coercion,
exploitation, or discrimination when completed. Ultimately, any
sustained effort requires both forms of advocacy, at which point the
question becomes: how might we support both?

Dilemmas like these force introspection about the role of researchers in
PAR and as infrastructure developers. Should researchers concentrate
efforts towards providing the most information (albeit limited in its
scope) in its most understandable form to the most workers as fast as
possible, or should infrastructure seek to facilitate larger-scale
inductive aggregate analyses which possess the potential for paradigm
shifts via strategic litigation, regulation, and ultimately better
policy outcomes – the goals of WIE? In this sense, the design of the
infrastructure can be reframed as a prioritization of stakeholders’
needs. Even so, each stakeholder’s contribution is just as necessary to
fulfilling any of the other’s goals as the next: the subject by
providing their data, WIE in aggregating the data for collective
advocacy, and researchers for development of the analytics systems,
defining what will result in the most agency for data subjects remains
muddled.

Undoubtedly, data subjects’ interests should come first. Selecting which
interests and how to serve them best is a more difficult question.
Furthermore, implementing this prioritization via data infrastructure
without cementing a single politics of change is not nearly so clear.
Our ultimate goal as researchers is to generate data architectures which
allow advocates with large-scale goals to shape policy and win rights
via collective advocacy, while also helping them seek immediate relief
and agency within poor working conditions. Building infrastructure that
does not overtly set priorities in pursuit of allowing both stakeholders
to access and analyze data autonomously also runs the risk of failing to
execute fully on either goal, potentially leading the effort astray from
the immediate needs of data subjects.^30^

The process of building infrastructures necessitates difficult
trade-offs: should these infrastructures seek to help data subjects
engage within the game set by the platform or should they seek to reveal
and change the rules through collective advocacy?

Achieving both of these goals requires simultaneously accommodating each
of the many, often conflicting requirements we have just enumerated.
Provided sufficient access to data, these goals do not need to be
mutually exclusive; no technical constraint prevents all of these
architectures to be implemented independently on top of a common source
of data. The resources and coordination needed to construct these
infrastructures are, however, desperately scarce. To make a case for
specific architectures that aspire to these goals, we inherently need to
make them and their governance as resource-efficient before also
critically considering what underlying politics we ourselves are at risk
of encoding into our own data infrastructures.

# Parallax 

Nick Srnicek points to a peculiarity that sets platform firms apart from
their predecessors: cross-subsidization – the unique ability of platform
companies to internally hedge individually unprofitable services on the
knowledge gained through the data they generate or other services they
facilitate.^31^ Gmail, Facebook, and of course Uber all fit this design
pattern. Gmail offers free email hosting in exchange for data used for
marketing or AI training. Facebook’s social network is likewise the
façade of a web-wise AdTech empire, while Uber consistently posts losses
in pursuit of squashing competition, logistics optimization, and even
autonomous vehicles.

Despite gains made in accessing the collective data which underpin these
systems, no institution, whether government, academic, or
public-interest, can realistically support data infrastructures that are
able to match the scale and sophistication of venture-backed platform
companies, promising boundless optimization and a future of AI – that
is, if they do so alone.

In the preceding sections, we considered the impacts of data structures
on the availability of information in data. First, we drew attention to
how data structures within DSAR responses obfuscated the information
contained in the data it communicated. Considering how data structure
inherently tailors the perception of underlying data based on the
politics and aims of its source systems, we critiqued the role played by
academics or others building underlying data infrastructures. We
concluded that any data institution meant to serve such diverse
stakeholders as WIE’s, and supported by resources pooled from data
subjects, activists, and academics, must avoid encoding similar
constraints on data. More specifically, this means being able to regard
data as a record of events in order to give clarity to data subjects, so
they can act with greater individual autonomy *within* a system where
information asymmetries left them without tools to resist. At the same
time, our infrastructure must also enable a critical lens on the very
same data, instead viewing it as trace of Uber’s system, the actions of
models operating on that system, and their diversion from workers’ and
advocates’ version of the truth. We recognize the complex and
contradictory nature of proposing a data analytics infrastructure
detached from any one analytical aim, while also supporting two
epistemic readings of the same information. In order to unpack this, we
borrow Žižek’s concept of the ‘parallax’ to account for both the
inherent conflicts that arise in designing this system.^32^ In optics
parlance, parallax refers to the phenomenon of observing equally
accurate movements of an object in the opposite directions caused by the
displacement between two points of view. In this sense, two measurements
can be both entirely accurate yet conflicting with one another only
because they are taken from two distinct perspectives.^33^

In Žižek’s *The Parallax View*, he reconsiders a basic Hegelian tenet –
the notion that analyses approaching the truth through a see-saw action
of contradicting thesis and antithesis, ultimately resolving in an
inevitable synthesis. Instead, Žižek abandons the need for any
resolution, and instead draws attention to the process of ‘putting two
incompatible phenomena on the same level’ where ‘the illusion of being
able to use the same language for phenomena which are mutually
untranslatable and can be grasped only in a kind of parallax view,
constantly shifting perspective between two points between which no
synthesis or mediation is possible’.^34^ Drawing examples from history
like those between economic conditions and political movements, or
between individual psychoanalysis and social dynamics, Žižek points his
readers’ attention to the ‘parallax gap, the confrontation of two
closely linked perspectives between which no neutral common ground is
possible’.^35^ For some truths or relationships taken as fact – such as
the relationship between individual psychoanalytic conditions and social
movements or between economic conditions and political conflicts – our
understanding exists in a certain tensile stasis. Each perspective is
untranslatable and fundamentally different yet somehow resolve as one
event (Figure 9.3).

Our choice of design for public-service data architectures resonates
with this framing. First, it accurately embodies our dilemma of
selecting which outcome (or form of solidary) our system should aspire
to – should it champion individual autonomy for workers *within* the
system or should it prioritize aggregate data for their collective cause
by working *against* that very same system? The parallax also resonates
with a confounding question around the epistemic lens with which we
might analyze data in the pursuit of empowering workers. Having pointed
to the unavoidable warping of meaning in data through its structuring,
can an architecture simultaneously use data from DSARs as evidence of
exploitation within a system *and* also show that the data that same
system produces is flawed, obfuscating or betraying the experience of
those operating within it? Put differently, can it champion solidarity
*within* Uber’s system through analysis of data, while using that same
data to critique that system’s own validity? Žižek’s operationalization
of the parallax offers that both are not only possible but also often
necessary within historical, philosophical, and scientific narratives.

Data subjects, activists, academics, and their respective funders see
the same data through different lenses. Some of these lenses do not
necessarily gaze towards a ground truth captured in data, but instead
critique the behaviours and intentions couched in the structural
artefacts left by prior manipulations

> ![](media/image1.png){width="2.6068853893263344in"
> height="4.899384295713036in"}

**Figure 9.3** Illustration of parallax

*Source*: Prepared by the authors based on Justin Wick’s example of
parallax, Wikimedia Commons,
https://commons.wikimedia.org/wiki/File:Parallax\_Example.png (accessed
12 December 2024).

and ontologies. In this sense, suitable analytics infrastructures must
be *parallax* in nature. That is, though relying on the same material
data as their basis, they must support inquiry which pursues divergent
epistemologies of the data and interpretations of autonomy.
Accommodating various perspectives is a significant challenge for any
analytical system, especially given such systems inherently adopt a
positivist viewpoint. Though relying on a common infrastructure may
offset some technical and organizational overhead, the admitted weakness
remains as to who maintains such systems and for what reward.

We posit that the best approach is not to conduct individual,
teleological efforts affirming a single perspective (and thus
structure), but rather architectures that can enable the diversity of
goals stakeholders seek and the epistemologies these investigations
require. In the next section, we describe the features of the
architecture we find best approximates this function given the technical
tools we possess today and the regulatory climate we operate within.

# Ways Forward: Architectures and Policy

You cannot buy a parallax data architecture from Amazon Web Services
(AWS) or fork one from GitHub (at least in name). We put forward,
however, that existing data analytics architectures used in open-source
and industry practice might be configured to embody many of the values a
parallax architecture might support. In this final section, we point to
examples of architectures and how we imagine data institutions might use
them to this end. Further, we place these technical systems in the
context of their regulatory climate – specifically pointing out the role
such architectures could play in the techno-legal ecosystems that new
data protection regulation has created. On the flip side, we also
describe the needs left unaddressed by today’s growing data protection
regimes but potentially aided by data institutions.

We started with an assumption: should data infrastructures be able to
lend transparency into their vastly more complex corporate counterparts,
they will need to pool resources and share knowledge as seamlessly as
the platforms integrate their ecosystems. We have argued that a primary
obstacle to this goal will be accommodating data structures which are
each independently necessary to analyse data for separate stakeholders
needs, but may also lead to conflicting demands on data infrastructures.

In our designs, we theorize that unstructured data analytics
infrastructures could provide a suitable technical basis to
simultaneously support the diverse analytical needs.^36^ When maintained
exclusively by a single academic or publicinterest institution, these
infrastructures may closely resemble current corporate practice, and
their cost might likewise become unjustifiable. In a shared setting,
however, the flexibility of unstructured architectures could allow
parties with common interests in underlying data but conflicting data
structures to still pool their resources and make them available as a
collective resource. This approach constitutes a departure from much of
the existing literature, which calls for strict data interoperability
standards from the outset.^37^ Instead, having considered
interoperability as something deeply contextual in its definition,
rather than a single objective format, we advocate for data institutions
to take up an unstructured approach to underlying data storage,
facilitating the maximum possibilities to query the same data resources,
without putting in place structures which obstruct other analyses.

Unstructured or NoSQL data architectures like Elasticsearch have a
variety of features which make them suitable for the demands of data
institutions. Most relevant to our discussion is their natural
orientation towards ‘schema on read’ (SoR) analytics strategies.^38^ SoR
systems stipulate that the greatest part of data structure is added at
time of analysis, rather than upon ingestion, while persistent data
remains in its unstructured form. While SoR is by no means a new idea,
it is rarely considered with a view respect to its potential impacts on
data stewardship and collective governance.

Pushshift is an excellent example of how unstructured data analytics can
be used at scale in the public service.^39^ The site maintains massive
repositories of comments and posts from Reddit and other social media
outlets as a research resource. Using an Elasticsearch architecture,
Pushshift makes data available via a search API. Elasticsearch’s
pre-indexing of data allows for data consumers to construct complex
searches, adding their own desired structure to data at the time of
their query with little latency, and the option to work iteratively,
without Pushshift needing to pre-compute statistics or add structures
which might obfuscate or prevent further analysis. The downside is that
more work may have to be done by the data consumer to extract their
desired information. Once this work is done the first time, however, it
is easy to replicate and build upon when queries are shared. In our
case, it is easy to imagine sharing a definitive query among
organizations for common metrics like pay-per-hour. Though Pushshift
demonstrates how a vast volume of data can be made available for many
purposes with relatively low overhead and maintenance cost (it is
maintained almost entirely by one person),^40^ its use case does not
contain sensitive personal data, and thus has not required the
implementation of collective or personal data governance controls as
platform worker data does.

Some of the natural resonance that unstructured data analytics systems
have with shared or collective governance originate in their
semi-decentralized architecture. Unstructured data analytics deployments
were engineered to rely on distributed data storage to facilitate
queries from many data analytics access points with different levels of
access, increasing data availability while limiting latency and actively
balancing workloads. Drastically simplifying their technical design,
technologies like Elasticsearch replicate data across isolated indexes
to reduce the time it may take to access any single record and to allow
multiple parties to simultaneously access the same data. The ‘horizontal
scalability’ lent by the distributed nature of these data stores means
different organizations, researchers, or even platforms could
independently contribute their data without fully relinquishing
governance over it.^41^ For example, WIE might maintain an index of
worker data controlled as a data trust through agreements with drivers
as they do today. WIE could make their index searchable by data
protection regulators in the UK, while an EU-based equivalent of WIE
might allow queries from WIE under a mutual agreement but block queries
from UK regulators. Similarly, the SoR stance of these architectures
would mean that stewardship decisions about anonymization or aggregation
could be made at the time of analysis, rather than being persistently
hard-coded into the functional structure of data stores. Queries from
particular parties could be limited to indexes or subsets of data; and
depending on their use or alternatively, data stewards could review the
results of queries submitted before allowing results to be returned.

Indexing data in unstructured data stores allows it to remain in its
original structure while also making it query-able for those consuming
it. At the same time, the effort placed into making information
available from it creates a tangible record of what is necessary to take
data from its original state into the necessary form for end users. We
have already seen an instance of how this might be useful to regulators
in our work with WIE. The code we created inherently chronicles a
running record of each deviation between DSAR responses we need to
resolve and the logs produced by our code record each time it is applied
to DSAR data, counting each row and field normalized and the frequency
of discrepancies between tables. For example, on each occasion a
timestamp was corrected from a human-readable time format to a
machine-readable format or vice versa, or the title of a column was made
to conform to other responses, a log was recorded. Logs like these could
be a crucial resource not only for authorities enforcing
interoperability requirements but also for pinning down what common data
formats should look like, or for tuning or training machine learning
models to automate the normalization of data formats we have thus far
performed manually. Other approaches to aggregating data from data
subjects for use in research and compliance also produce similar
artifacts. The Open-Source Data Donation Framework or (OSD2F) elicits
scripts from researchers to be tested in the private environment of a
data subject’s browser before allowing data donors to elect to
contribute their data to research.^42^ The scripts contributed by
researchers both play a similar role to logs we produced, showing the
necessary transformations to make data interoperable, and the queries we
mentioned earlier, by providing open-source or shared resources for
extracting information from the underlying data.

There are also undoubtedly weaknesses of relying on unstructured data
analytics technologies. One aspect is that they are only
semi-decentralized when compared to other, fully decentralized
alternative data architectures. Tim BernersLee’s Solid project (to which
our team actively contributes) facilitates one-off permissions to data
held by subjects, making it possible for data to be accessed by services
without ever leaving the data subject’s personal data store.^43^ Solid
envisions a future in which data stored in a decentralized setting is
organized according to a common semantic format (Resource Description
Framework, or RDF), allowing for perfect interoperability. The price of
Solid’s decentralization is strict adherence to this common data format.
We see unstructured data infrastructures not as competing with such
decentralized ecosystems but as a layer which might enhance them. If (or
until) such adoption is achieved, we see unstructured data analytics
deployments as a necessary bridge to ease the pains of data
normalization and deliver needed analytical insight now. Indeed,
subjects might consent to share data directly from their Pod with a data
institution which has a governance regime complementary to their values.
Sylvie Delacroix and Neil D. Lawrence imagine a similar techno-legal
configuration when they describe ‘a plurality of bottom-up data trusts’,
meant to suit the highly heterogeneous sets of data subject preferences
– something they viewed as an obstacle to the initial data trust model
proposed by Lilian Edwards and championed by Dame Wendy Hall and Jérôme
Pesenti.^44^

One of the inherent disadvantages to the model we propose is its
reliance on DSARs for its data. Much of our earlier sections covered
specifically how access to data via DSARs does not necessarily lead to
the transparency or agency sought from aggregating it. This point
becomes even more critical in the context of new regulations that grant
more direct research access to platform data for researchers. The added
access granted by Article 40 of the EU’s DSA constitutes a significant
advance in data access for evaluating systemic harms and risks of the
type we examine in our work with WIE.^45^ This provision of the DSA is
unfortunately not applicable to Uber as it does not break the
45-million-user thresholds set by the policy.^46^ With laws like the DSA
opening new avenues to aggregate data access and recent cases won by WIE
establishing a precedent in which Uber cannot deny data access for the
purpose of aggregation, we might expect obfuscation through the use of
data structure to become an even more common tactic of data controllers.
Remaining optimistic, however, the added access researchers may be able
to achieve for other platforms via the DSA could also become a critical
resource to enhance data institutions drawing from aggregated DSAR
responses. The vastly different nature of this data – likely aggregate,
higher velocity (more regularly refreshed), and hopefully more readily
machine readable – only strengthens the need of architectures that can
quickly accommodate the combination or comparison of differing data
structures with existing data collected directly by data subjects
through their own self-tracking or through DSARs.

In the absence of greater legal tools to access data, grassroots efforts
have also been successful in sourcing data to give workers immediate
insights and audit the behaviour of algorithms. Dan Calacci and Alex
Pentland creatively combined a chatbot with computer vision techniques
to collect and process screenshots of workers for the US platform
Shipt.^47^ Through this technique, the authors worked with data subjects
and activists to reveal how alterations to the design of dynamic pay
systems on the part of the platform resulted in changes to the wages of
workers. Commercial implementations that source data directly from
individual workers have also emerged such as Argyle, a service that uses
workers’ credentials to fetch their data and build verifiable labour
records across platforms. Rodeo, an app that allows workers to compare
gig-work offers across platforms, uses Argyle to source data, but is
ultimately at risk of losing access to data should platforms cut off
data flows as Deliveroo, a UK-based food delivery platform, has recently
done.^48^

# Conclusion

The technological innovation that has facilitated platform dominance
could also be used to supplant the information asymmetries it has
created. Unfortunately, platforms’ aggregation of data and the powerful
algorithmic technologies that emerge from it are cumulative in their
momentum, and they have been given a multi-billion-dollar head start.
Further, hegemonic patterns of control have also made institutions in
academia, civil society, and government slow to adequately retool and
cooperate to reverse escalating concentrations of power.

Regulation, however, is beginning to catch up, creating cracks in the
veil between data subjects’ and controllers’ views of the systems on
which they both rely. Further, new generative AI methods and analytics
architectures, though conceived to power companies’ data-grabs, could be
put to use to erase much of the overhead that separates platforms’
technical capabilities from those of organizers who seek to hold them to
account. While some regulations like the DSA might help organizers catch
up in the analytics race through better data access and mandated
algorithmic transparency, others also slow down or limit the analytics
practices that set platforms apart. The Digital Markets Act (DMA), 2022,
prevents large platforms from pooling data sourced from disparate
services undercutting or disincentivizing ‘cross-subsidization’.

Together, newfound access to data, combined with prohibitions of
platforms’ data pooling practices, presents a distinct opportunity for
advocacy organizations and research bodies to produce sustainable
alternatives that are also accountable to data subjects. Despite this
promising shift in the regulatory landscape, the most treacherous
obstacles for organizers may soon come not from barriers to accessing
data or technology but from understanding how to redraw deeply
intrenched institutional boundaries, while also including data subjects
to participate in shifting power.

# Notes

1.  Rob Kitchin and Gavin McArdle, ‘What Makes Big Data, Big Data?
    Exploring the Ontological Characteristics of 26 Datasets’, *Big Data
    and Society* 3, no. 1 (2016), DOI:
    https://doi.org/10.1177/2053951716631130.

2.  A whole sub-industry has sprung up not only offering data analytics
    as a service but also in the optimization of organizational
    structures surrounding analytics development in ‘AI operations’
    (AIOps). So-called process-mining tools have also become widely
    available to streamline data structuring, pipeline building, and
    exploratory analysis by non-technical users. See Yingnong Dang,
    Qingwei Lin, and Peng Huang, *AIOps: Real-World Challenges and
    Research Innovations*, 2019 IEEE/ACM 41st International Conference
    on Software Engineering: Companion Proceedings (ICSE-Companion)
    (Institute of Electrical and Electronics Engineers, 2019),
    https://ieeexplore. ieee.org/document/8802836 (accessed 28 February
    2023).

3.  Dan Calacci, ‘Organizing in the End of Employment: Information
    Sharing, Data Stewardship, and Digital Workerism’, 2022 Symposium on
    HumanComputer Interaction for Work, Durham, NH, 2022.

4.  Jack Hardinges and Jared Robert Keller, ‘What Are Data Institutions
    and Why Are They Important?’ Open Data Institute, 29 January 2021,
    https://
    theodi.org/article/what-are-data-institutions-and-why-are-they-important
    (accessed 7 November 2022).

5.  Hardinges and Keller, ‘What Are Data Institutions’.

6.  Lilly C. Irani and M. Six Silberman, ‘Turkopticon: Interrupting
    Worker Invisibility in Amazon Mechanical Turk’, Proceedings of the
    SIGCHI Conference on Human Factors in Computing Systems, Association
    for Computing Machinery, 2013, https://dl.acm.org/
    doi/10.1145/2470654.2470742 (accessed 13 July 2022).

7.  Jack Hardinges and Jared Robert Keller, ‘What Are “Bottom-Up” Data
    Institutions and How Do They Empower People? – the ODI’, Open Data
    Institute, 25 June 2021,
    https://theodi.org/article/what-are-bottom-up-datainstitutions-and-how-do-they-empower-people
    (accessed 7 July 2021).

8.  Tobias Fiebig, Seda Gürses, Carlos H. Gañán, Erna Kotkamp, Fernando
    Kuipers, Martina Lindorfer, Menghua Prisse, and Taritha Sari, ‘Heads
    in the Clouds: Measuring the Implications of Universities Migrating
    to Public Clouds’, 27 July 2021, http://arxiv.org/abs/2104.09462
    (accessed 20 June 2022).

9.  Fiebig, Gürses, Gañán, Kotkamp, Kuipers, Lindorfer, Prisse, and
    Sari, ‘Heads in the Clouds’.

10. Wendy Hall and Jérôme Pesenti, ‘Growing the Artificial Intelligence
    Industry in the UK’, Department for Digital, Culture, Media and
    Sport and Department for Business, Energy and Industrial Strategy,
    GOV.UK, 2017,
    https://www.gov.uk/government/publications/growing-the-artificialintelligence-industry-in-the-uk
    (accessed 11 November 2024).

11. René Mahieu and Jef Ausloos, ‘Recognising and Enabling the
    Collective Dimension of the GDPR and the Right of Access’, preprint,
    29 April 2020, https://osf.io/b5dwm (accessed 29 October 2021).

12. Dan Calacci and Jake Stein, ‘From Access to Understanding:
    Collective Data Governance for Workers’, *European Labour Law
    Journal* 14, no. 2 (2023), DOI:
    https://doi.org/10.1177/20319525231167981.

13. Worker Info Exchange (WIE) is a non-profit data rights and worker
    advocacy organization in the United Kingdom (UK). The organization
    assists workers with individual claims, including algorithmic
    discrimination, data access, unfair working conditions, and unjust
    dismissals. Closely aligned with the App Drivers and Couriers Union
    (ADCU), the organization is active in collective advocacy, winning
    several landmark cases establishing standards for data access in the
    UK and the European Union (EU). For information about WIE, visit
    workerinfoexchange.org.

14. Our project regards data autonomy first and foremost as data
    subjects’ ability to control, manage, and maintain their personal
    data encompassing both personal data privacy and transparency into
    how data is used and processed. We also consider data autonomy to go
    beyond these core pillars of data governance to include data
    subjects’ access to ‘mutual legibility’, or the ability for data
    subjects to understand data in the same contexts (aggregate and
    individual) as data collectors.

15. *Applicants 1-4 v. UBER BV* \[2023\] Rechtbank Amsterdam
    200.295.742/01; *Applicants 1-6 v. UBER BV* \[2023\] Rechtbank
    Amsterdam 200.295.747/01.

16. ‘AWO’, https://awo.agency (accessed 31 May 2023).

17. This research project has been approved by the Departmental Research
    Ethics Committee for Computer Science, University of Oxford, under
    reference CS\_C1A\_23\_016\_001.

18. Britt S. Paris, Corinne Cath, and Sarah Myers West, ‘Radical
    Infrastructure: Building beyond the Failures of Past Imaginaries for
    Networked Communication’, *New Media and Society* 26, no. 11 (2023),
    DOI: https:// doi.org/10.1177/14614448231152546.

19. Slavoj Žižek, *The Parallax View* (paperback) (MIT Press, 2009
    \[2006\]).

20. See Tyler Akidau, Robert Bradshaw, Craig Chambers, Slava Chernyak,
    Rafael J. Fernández-Moctezuma, Reuven Lax, Sam McVeety, Daniel
    Mills, Frances Perry, Eric Schmidt, and Sam Whittle, ‘The Dataflow
    Model: A

> Practical Approach to Balancing Correctness, Latency, and Cost in
> MassiveScale, Unbounded, Out-of-Order Data Processing’, *Proceedings
> of the VLDB Endowment* 8, no. 12 (2015): 1792–1803. For example, an
> analytics system to evaluate the performance of a jetliner will
> introduce structure early on in the pipeline in order to monitor
> complex machine-generated data in real time whereas social media
> analytics systems might introduce structure later in the pipeline to
> allow for inductive analysis.

1.  Finn Brunton and Helen Fay Nissenbaum, *Obfuscation*: *A User’s
    Guide for Privacy and Protest* (MIT Press, 2015),
    http://public.eblib.com/choice/ publicfullrecord.aspx?p=4093096
    (accessed 3 December 2020).

2.  Jef Ausloos and Pierre Dewitte, ‘Shattering One-Way Mirrors: Data
    Subject Access Rights in Practice’, *International Data Privacy Law*
    4, no. 8 (2018): 4–28.

3.  EU General Data Protection Regulation (GDPR), 2016, Article 4.

4.  *Applicants 1-4 v. UBER B.V.; Applicants 1-6 v*. *UBER B.V*; Paris,
    Cath, and West, ‘Radical Infrastructure’. Please note the research
    described in this article occurred prior to the conclusion of these
    cases.

5.  Jessica Phillips, ‘How Uber’s Dynamic Pricing Model Works’, *Uber
    Blog*, 21 January 2019,
    https://www.uber.com/en-GB/blog/uber-dynamic-pricing (accessed 31
    May 2023).

6.  Geoffrey C. Bowker, *Memory Practices in the Sciences* (MIT Press,
    2005); Yanni A Loukissas, *All Data Are Local: Thinking Critically
    in a Data-Driven Society* (MIT Press, 2019).

7.  Alex Bowyer, Jessica Pidoux, Jacob Gursky, and Paul-Olivier Dehaye,
    ‘Digipower Technical Reports: Auditing the Data Economy through
    Personal Data Access’, Zenodo, https://zenodo.org/record/6554178
    (accessed 7 October 2022).

8.  Paris, Cath, and West, ‘Radical Infrastructure’.

9.  Veena Dubal, ‘Wage Slave or Entrepreneur? Contesting the Dualism of
    Legal Worker Identities’, *California Law Review* no. 105 (2017):
    65–123.

10. Paris, Cath, and West, ‘Radical Infrastructure’.

11. Nick Srnicek and Laurent De Sutter, *Platform Capitalism* (Polity
    Press, 2017).

12. Žižek, *The Parallax View*.

13. Kaj Strand, ‘Parallax’, *Encyclopedia Britannica*, 2023,
    https://www.britannica.

> com/science/parallax (accessed 12 December 2024).

1.  Žižek, *The Parallax View*.

2.  Žižek, *The Parallax View*.

3.  Rick Cattell, ‘Scalable SQL and NoSQL Data Stores’, *ACM SIGMOD
    Record* 12, no. 39 (2011): 12–27.

4.  Gianclaudio Malgieri and Frank Pasquale, ‘From Transparency to
    Justification: Toward Ex Ante Accountability for AI’, Brooklyn Law
    School, Legal Studies Paper 712, 2022, 27; Milagros Miceli, Tianling
    Yang, Adriana Alvarado Garcia, Julian Posada, Sonja Mei Wang, Marc
    Pohl, and Alex Hanna, ‘Documenting Data Production Processes: A
    Participatory Approach for Data Work’, 9 August 2022,
    http://arxiv.org/abs/2207.04958 (accessed 12 August 2022).

5.  Sladjana Jankovic, Snezana Mladenovic, Dušan Miodrag, and Mladenović
    Slavko Vesković, ‘Schema on Read Modeling Approach as a Basis of Big
    Data Analytics Integration in EIS’, *Enterprise Information Systems*
    1180, no. 12 (2018): 1–22.

6.  Jason Baumgartner, Savvas Zannettou, Brian Keegan, Megan Squire, and
    Jeremy Blackburn, ‘The Pushshift Reddit Dataset’, *Proceedings of
    the International AAAI Conference on Web and Social Media* 14, no. 1
    (2020): 830–839.

7.  ‘Contributors to Pushshift/Api’,
    https://github.com/pushshift/api/graphs/ contributors (accessed 31
    May 2023).

8.  Venkat N. Gudivada, Dhana Rao, and Vijay V. Raghavan, ‘NoSQL Systems
    for Big Data Management’, 2014 IEEE World Congress on Services,
    Institute of Electrical and Electronics Engineers, 2014,
    https://ieeexplore.ieee.org/ document/6903264 (accessed 28 February
    2023).

9.  Slađana Janković, Snežana Mladenović, Dušan Mladenović, Slavko
    Vesković, and Draženko Glavić, ‘Schema on read Modeling Approach as
    a Basis of Big Data Analytics Integration in EIS’, *Enterprise
    Information Systems* 12, no. 8–9 (2018): 1180–1201.

10. Essam Mansour, Andrei Vlad Sambra, Sandro Hawke, Maged Zereba,
    Sarven

> Capadisli, Abdurrahman Ghanem, Ashraf Aboulnaga, and Tim BernersLee,
> ‘A Demonstration of the Solid Platform for Social Web Applications’,
> Proceedings of the 25th International Conference Companion on World
> Wide Web, 2016, 223–226.

1.  Sylvie Delacroix and Neil D. Lawrence, ‘Bottom-Up Data Trusts:
    Disturbing the “One Size Fits All” Approach to Data Governance’,
    *International Data Privacy Law* 9, no. 4 (2019): 236–252; Lilian
    Edwards, ‘The Problem with Privacy’, *International Review of Law
    Computers and Technology* 18, no. 3 (2004): 263–294; Hall and
    Pesenti, ‘Growing the Artificial Intelligence Industry in the UK’.

2.  Martin Husovec and Irene Roche Laguna, ‘Digital Services Act: A
    Short Primer’, 2022, DOI: https://dx.doi.org/10.2139/ssrn.4153796.

3.  ‘Uber’, https://www.uber.com/legal/de/document (accessed 31 May
    2023).

4.  Dan Calacci and Alex Pentland, ‘Bargaining with the Black-Box:
    Designing and Deploying Worker-Centric Tools to Audit Algorithmic
    Management’, *Proceedings of the ACM on Human-Computer Interaction*
    1, no. 6 (2022): 1–24.

5.  Oscar Hornstein, ‘Deliveroo Accused of Blocking Courier Access to
    Gig Economy Finance App’, *UKTN*, 21 March 2023,
    https://www.uktech.news/ mobility/deliveroo-blocks-rodeo-20230321
    (accessed 31 May 2023).
