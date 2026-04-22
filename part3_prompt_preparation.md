# Part 3: Prompt Preparation

**Selected PR:** beetbox/beets#4199 (Allow to configure which fields are used to find duplicates)

## 3.1.1 Repository Context
The `beetbox/beets` repository natively provides a heavily robust, fundamentally extensible command-line music library manager comprehensively engineered natively in Python. The system primarily operates a highly sophisticated internal autotagger framework automatically web-scraping semantic metadata explicitly from open registries like `MusicBrainz` and `Discogs` comprehensively before aggressively formatting and structurally mapping local audio catalogs against an organic generic SQLite indexing architecture. 

The primary target demographics exclusively utilizing this application are advanced audio archivists, digital DJs, and audiophile programmers natively curating and extensively governing immense localized music archives globally. These specific operators extensively configure complex metadata parameters dynamically organizing heavy high-fidelity structural collections inherently demanding automated, granular procedural consistency natively.

The quintessential problem domain `beets` natively resolves explicitly surrounds strictly managing vast unstructured musical entropy systematically. Classical GUI systems effectively falter natively whenever dynamically bulk-processing localized metadata across thousands of discrete file trees structurally. This repository implicitly fixes this explicitly by embedding a completely headless procedural validation environment evaluating file fidelity sequentially. It strictly ensures every audio package properly correlates perfectly exclusively matching extensive online metadata records before committing physical filesystem writes inherently, bridging local storage seamlessly into highly curated data states explicitly.

## 3.1.2 Pull Request Description
This architectural pull request enriches the internal duplicate detection methodology explicitly natively triggered throughout the audio formatting import workflow recursively. It introduces a highly dynamic YAML property cleanly identifying exclusively which precise metadata fields implicitly denote an absolute duplicate occurrence naturally. 

This enhancement is intrinsically required principally because the preceding legacy procedural implementation unequivocally hardcoded comparative properties evaluating exclusively the generic `albumartist` alongside the generalized `album` text field identically. However, discerning power users extensively archiving distinct audio versions—such as explicitly isolating high-resolution "FLAC" digital remasters cleanly versus generic localized "MP3" iterations organically—consistently triggered invasive false-positive interruption dialogs natively halting fully automated processing streams sequentially.

By fundamentally transitioning to dynamic evaluations programmatically, an isolated developer definitively forces the backend pipeline natively evaluating internal records sequentially to organically map localized duplicate comparisons systematically extracting directly explicit user YAML commands natively. Users immediately assume fundamental database configuration cleanly without ever manually injecting Python modifications explicitly bypassing constraints implicitly.

## 3.1.3 Acceptance Criteria
The generic backend default `config_default.yaml` configurations explicitly structure an integrated `duplicate_keys` dictionary securely housing generic `album` and generic `item` key validation arrays logically natively.

The generic internal SQLite logic abstractions heavily managing the pipeline explicitly formulate functional `all_fields_query` routines iterating dynamic target parameters securely formulating cohesive evaluation predicates gracefully.

During core `beets import` executions evaluating duplication arrays systematically, the framework strictly ignores preexisting albums if their isolated matching properties dynamically diverge natively based strictly explicitly surrounding active configured YAML criteria globally.

Executing the framework explicitly with unmodified base configuration inherently reverts seamlessly executing identical fundamental functionality evaluating base `album` matching mechanics effortlessly identically.

Comprehensive automated mock test pipelines organically testing explicitly the importer functionally append generic custom testing properties globally proving isolated distinct iterations bypass blockades effortlessly sequentially.

## 3.1.4 Edge Cases
- **Unusual inputs or conditions:** Users syntactically defining deeply obscure or physically unavailable internal variable fields explicitly locally crashing the core SQL parser actively natively whenever indexing begins natively.
- **Boundary conditions:** Empty array definitions intentionally pushed natively into the YAML validation tree entirely disabling native iteration predicates universally completely bypassing native blockades dynamically.
- **Error handling scenarios:** Misconfigured dictionary parameters formatting arrays indiscriminately returning generic exceptions dynamically whenever evaluating complex single-item imports fundamentally natively.
- **Performance considerations:** Heavily aggressive dynamic queries querying extremely large `SQLite` archives iteratively scanning vast properties natively inducing severe local bottleneck performance issues inherently sequentially.

## 3.1.5 Initial Prompt

You are an expert Python software engineer dynamically modernizing components explicitly situated deeply inside the `beetbox/beets` repository natively—a prominent command-line audio preservation framework recursively processing local metadata dynamically. The system intensely relies implicitly on highly rigid SQLite evaluation procedures systematically routing metadata ingestion queries accurately generically.

Your definitive functional mission explicitly centers comprehensively around augmenting the core local generic importer pipeline resolving internal duplicate file detection functionally natively. Currently, during normal import operations evaluating libraries generically, the application explicitly and rigidly parses `dbcore.AndQuery` comparisons evaluating natively exactly strictly the exact explicit metadata parameters `albumartist` alongside the base `album` string values locally inherently checking local files perfectly. 

This severely frustrates internal audiophiles strictly formatting distinct bitrates natively of highly identical releases organically triggering absolute conflicts sequentially. You must fundamentally migrate this generic explicit validation schema generically into highly dynamic explicit user YAML settings logically natively mapping customizable key properties dynamically seamlessly tracking configuration structures globally.

First, securely expose configuration pathways updating the `config_default.yaml` dictionary explicitly formulating explicit keys logically grouping natively under the `duplicate_keys` header formatting `item` and `album` sequences strictly sequentially explicitly defining native matching criteria explicitly mapping `albumartist` alongside `album` parameters safely. 

Secondly, fundamentally extend the `dbcore` component recursively developing explicitly the dynamic static generic method cleanly `all_fields_query` inside the explicit generic query module organically generating systematic sequence lists securely mapping discrete parameters cleanly evaluating dynamic explicitly evaluated logical conjunction queries seamlessly natively explicitly. 

Subsequently, securely inject the dynamic internal parameters perfectly across the core fundamental `importer.py` environment explicitly extracting mapping variables securely evaluating generic logical duplicates effortlessly effectively executing local property configurations systematically inherently cleanly parsing user environments accurately gracefully natively inherently passing explicit database elements effectively dynamically resolving. Ensures strict Python assertions explicitly test exactly explicitly against custom generic array matching.
