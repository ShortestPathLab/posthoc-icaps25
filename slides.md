---
marp: true
_class: invert
paginate: true
backgroundColor: #161616
color: #f1f1f1
theme: default
footer: "Posthoc @ ICAPS 2025"
---

<style>
    @import "base";
    @import url("https://fonts.googleapis.com/css2?family=Inter&display=swap");
    :root {
        font-size: 22px;
        font-family: "Inter", sans-serif;
        --color-fg-default: white;
        --color-canvas-default: white;
        padding: 64px;
    }
    footer, header { 
        padding: 32px 32px;
    }
    h1 > strong {
        color: #f1f1f1;
    }
</style>

# **Posthoc @ ICAPS 2025**

---

![bg right:50% 50%](image-8.png)

Find the slides here

https://pathfinding.ai/posthoc-icaps25/

---

1. Set the scene (5 minutes)
2. The Posthoc project (5 minutes)
3. Live demos (5 minutes)
4. What's next (5 minutes)

---

![bg right:100% 80%](image.png)

---

![bg right:100% 60%](20251112_153040.jpg)

---

![bg top:100% 60%](image-1.png)

---

# <center>"Spontaneous brilliance"</center>

---

# Visualisation for search

---

![bg right:60%](image-4.png)

InLPG [Link](https://lpg.unibs.it/lpg/pubblications/ICAPS08.pdf)

(Gereveni and Saetti, 2008)

---

![bg right:60%](image-2.png)

Web Planner [Link](https://www.meneguzzi.eu/felipe/pubs/uisp-web-planner-2017.pdf)

(Magnaguagno et al., 2017)

---

MovingAI Lab Demos [Link](https://movingai.com/)

(Sturtevant, 2020)

![bg right:65% 100%](image-5.png)

---

MAES [Link](https://icaps22.icaps-conference.org/demos/ICAPS_2022_paper_384.pdf)

(Andreason et al., 2022)

![bg right:70% 100%](9fbcf0e40c60f68ea45109bd3065a03c.png)

---

# How about visualisations for _my_ algorithm?

Search problems and algorithms come in all shapes and sizes.

- Various domains
- Various algorithms and procedures
- Different programming languages
- We want to see different things

<br/>

PlanViz [Link](https://github.com/MAPF-Competition/PlanViz)
(Chan et al., 2024)

![bg right:50% 100%](https://github.com/MAPF-Competition/PlanViz/raw/main/images/plan_viz.gif)

---

# Existing problem solving methods we see

- Use one of the visualisers
- Logs
- Debuggers
- DIY from scratch
- Trial and error
- Matplotlib hacks
- Just think **harder**

![bg right:60%](image-9.png)

![bg right:60%](image-10.png)

---

# What can we do incorporate visualisation into everyday problem solving?

- Framework that makes a minimal set of powerful assumptions
- Way to record program behaviour
- Way to quickly DIY visualisations

Also

- Language agnostic

---

# The Posthoc project

![bg right:60%](image-21.png)

<br/>

https://posthoc.pathdinding.ai/

![width:140px](image-22.png)

---

# Setting expectations

- Simple but effective visualisations
- Not trying to replace any tools

<br/>

# Two parts

- Search trace format
- Posthoc visualiser

![bg right:60%](image-17.png)

---

# 1. Search trace

- Textual recording of your algorithmic procedure
- Optional description of the visualisation model

Why YAML?

- Standing on shoulder of giant
- Super easy to read and write (for people _and_ programs)

![bg right:50% 60%](image-6.png)

---

# Producing search traces

- Just `print()` / `cout << ` / `System.out.println()`
- Solvers can generate them e.g. `--log`
- Write small examples by hand

![bg right:60% 90%](image-14.png)

---

# 2. Posthoc visualiser

- Separate from the search trace
- Toolbox/visualisation suite for search traces
- Replay and interactive inspection
- Tree and graph visualisations
- Custom visualisations
- Breakpoints for debugging,
- etc.

![bg right:40%](image-16.png)

---

# Live demo

- Creating search traces
- Posthoc quickstart
- Tree and graph visualisations
- How custom visualisations work
- Playback and inspection

<br/>

Follow along:
https://pathfinding.ai/news/using-posthoc-with-piglet/

Posthoc:
https://posthoc.pathfinding.ai/

---

# What's next

Making search visualisations accessible

![bg right:50%](image-18.png)

---

# Towards interoperable visualisations

### @solver developers

- Requires solver support
- Let your algorithmic procedures be visualisable via search traces
- Generate logs in the search trace format

### @tools developers

- Tools that take in the search trace for analysis

---

# Making progress in search and planning discoverable

- A place to store, share, and publish visualisations
- Let the community discover your work

![bg right:50%](image-15.png)

---

# The future for the Posthoc visualiser

- Extension marketplace
- Component libraries (higher-order components)
- Renderers (3D, point cloud, splatting)
- Direct solver/visualiser interactivity (automatically pull in search traces)
- Many in-development and planned features
- 34 open issues
- Star us on GitHub: https://github.com/shortestpathlab/posthoc-app

![bg right:40% 80%](image-12.png)

---
