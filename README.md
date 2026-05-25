## Elk Hunting Study: Calling, Shot Opportunity, and Recovery

This project is an attempt to better understand what actually leads to success in elk hunting.

There is a lot of advice out there—when to call, where to be, how far to shoot—but most of it is based on personal experience. The goal here is to collect structured data from real hunters in the field and see what patterns show up. 

### The study follows hunters through the full sequence of a hunt:

Setup → Elk response → Encounter → Shot opportunity → Shot → Recovery

Instead of focusing on just one part of the hunt, the idea is to understand how each step connects to the next.

--------------------------------------------------

### What This Project Is Trying to Answer

#### There are three main questions:

1. When are elk most likely to respond?
   Looking at things like time of day, elevation, calling method, and hunting pressure.

2. What turns a response into a real opportunity?
   Not every bugle turns into a shot. This part examines what distinguishes the setups that lead to encounters from those that don’t.

3. What leads to a successful recovery after a shot?
   Focusing on shot distance, angle, hit location, and decisions made after the shot.

There is also a comparison between archery and rifle hunters, but that’s treated as one factor among many, not the main focus.

--------------------------------------------------

### How the Data Is Collected

#### Hunters in the study log three types of events:

1. Hunter Profile (Via Google Forms)
Basic information about experience level, hunting style, and equipment.

2. Setup / Calling Logs (Via Onx)
Each time a hunter stops to call, glass, or listen, they record:
- Location (via OnX)
- Time and elevation
- How did they call (bugle, cow call, etc.)
- Whether elk responded
- Whether it led to an encounter or a shot opportunity

3. Shot Reports (Via OnX)
If a shot is taken, additional details are recorded:
- Shot distance and angle
- Hit location (if known)
- Whether the animal was recovered
- Distance traveled after the shot

The goal is to keep data collection realistic so it doesn’t interfere with the hunt.

--------------------------------------------------

### Project Structure

elk_hunter_study/

data/
  raw/        # original logs and exports
  interim/    # cleaned and validated data
  processed/  # modeling datasets
  final/      # final datasets and summary tables

notebooks/
  data_review.ipynb
  cleaning_validation.ipynb
  exploratory_analysis.ipynb
  model_call_response.ipynb
  model_shot_opportunity.ipynb
  model_recovery.ipynb

scripts/
  data cleaning and transformation scripts

outputs/
  figures/
  tables/
  maps/
  final_report/

--------------------------------------------------

### Approach

The analysis is broken into three parts:

1. Calling Response Model
Look at what factors increase the probability of getting an elk response.

2. Shot Opportunity Model
Look at what factors increase the chance that a response leads to a shot opportunity.

3. Recovery Model
Look at what factors influence whether a shot animal is recovered.

The idea is not just to build predictive models, but to understand which variables actually matter.

--------------------------------------------------

#### Why This Matters

A lot of hunting advice is based on small sample sizes—one hunter, one season type, one unit.

This project tries to:
- Combine data across many hunters
- Separate opinion from patterns
- Identify what actually moves the needle

If done right, it should give practical takeaways like:
- When to spend more time calling vs moving
- What kind of setups are most productive
- How shot decisions impact recovery

--------------------------------------------------

#### Limitations

This is field data, not a controlled experiment.

Things to keep in mind:
- Hunters vary in skill and decision-making
- Not all variables can be measured (elk behavior, pressure, etc.)
- Shot sample size will likely be smaller than setup data
- Some data will be self-reported and imperfect

The goal is not perfect accuracy, but useful directional insight.

--------------------------------------------------

#### Future Ideas

- Add weather API integration
- Automatically enrich GPS points with terrain data (slope, aspect, distance to roads/water)
- Build a live dashboard for in-season insights
- Expand on 2026 findings for 2027

--------------------------------------------------

#### Contributing

If you’re a hunter interested in participating or improving the data collection process, feel free to reach out or open an issue.

--------------------------------------------------

#### Authors: 
Elk Nerd       -- Project Lead     
Lance Santerre -- Lead Data Scientist
