# What are we building?

Pixels to cosmology. 

Broadly speaking, we need
1. a pixel calibration pipeline
2. a photometric and spectroscopic extraction pipelines, and 
3. a SN cosmology catalog pipeline. 
This will also include adjacent software, such as simulation tools, development and production environments, and community support interfaces.

We will build a single pipeline repo/package that uses pinned requirements and `from package import *` in __init__.py files. This way, we can add packages/algorithms that we do not managage nor maintain. As apart of the PIT contract, we will provide a collection of sufficent packages that the pipeline can depend on, but we also know that these specific packages won't always be the best option for every analysis.

## Current tools we can repurpose

- DES/See-Change SMP - Photometry
- Linear/Axe/Grizzly - Spectroscopic extraction
- SNANA/PIPPIN - catalog pipeline
- SCONE - photometric typing

## We need a tool for

- spectroscopic typing
- redshift measurements
- data management (keeping track of files, building catalogs, ...)
- a meta tool (like PIPPIN) but includes more detailed data prep stages, can be module in what it calls and where it runs, and maybe more.


# How we building things

## Practical Processes

### Starting:

1. We will create a long list of what we can do.
1. Prioritize list.
1. Set out to create (and complete) a small collection of tasks over one month

We will use a dedicated repo (not a pipeline repo) for collecting, "sizing", describing done state, and prioritizing backlog issues. We will use a GitHub project, one per month, to track that month's tasks. - Can we put this at the top of the todo list? Add a link to the filtered view from the GitHub org's homepage.

### While working:

- Check-in daily (via slack) stating what we got done yesterday, what we plan to do today, and if there is anything "blocking" your progress.
- Person TBD will attempt to remove blocks/hurtles in order to allow for improved productivity.

Mark issues as done by moving to done column in sprint, applying done tag, and closing issues. If issue is connected to a pipeline (calibration, photometry, spectral extraction, cosmology-catalog stage), then ..??.. connect pipeline issues/PR with project planning issues.

### At end of month:

- Present what we have made and celebrate that progress!
- Evaluate what tools and processes worked and did not work (communication, access, chairs, software, ...)
- Check the backlog of tasks: add new items, remove unneeded items, and reprioritize
- Make adjustments to process and priority list
- Repeat by slecting the next month's set of tasks.
	
	
## Meta Processes

We can always get better.
	- Code review procedures (link to this document)
	- DEI training (link to this document)
	- Monthly retrospective reviews

We respect and include everyone.
	- Inclusion plan (link to this document)
	- Code of conduct (link to this document)
	- DEI training (link to this document), ...
	- 

We will deliver one modular and flexible pipeline
	- We code in similar style and not something that reads like a new person wrote each "paragraph."
	- Task definitions need to include discussion of implementation and integration into the pipeline as a whole.
	- We use a consistent code style guide and/pr an automatic code formatter (link to this document)
	- CI: checks formatting, checking regression tests, checking documentation, ... (link to this document)
	- Code review (link to this document) to check logic and ensure more than 1 person knows/has seen each aspect of the code.

Pipeline features will be user focused
	- We will determine our task by working through them as a user wants to do "specific action". In order to do this, we will build y as a function/class/new pipeline.

We avoid leaving things half-done. Started is not a useful state, but knowing what people are *actively* working on is useful information.
	- Make smaller, more easily completable tasks
	- Work in longer uninterrupted blocks of time
	- Work with a partner to tackle larger issues.
	- Try not to leave things started but not done. Don't split your focus on multiple tasks.

