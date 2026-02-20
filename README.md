# Emergency Callbox Optimization

## Project Overview

Situated around the McGill campus are emergency callboxes. These are installed and maintained by the McGill security team to help students and the general public get help in case of an emergency. They can be spotted by their bright colours and blue light attached to them. Some of these phones are outdated or in suboptimal locations and it would be beneficial for the McGill security team to optimize their location and type. Note: since the widespread use of mobile phones these boxes have shifted more to a general-purpose security element. They provide bright light and surveillance to many areas of campus and are constantly monitored by the security team on campus. This can be framed as an linear programming optimization problem where the aim is to minimize cost subject to a percent of campus covered by the boxes. See the photo below for an example callbox.

### Example Photo
<p align="center">
  <img src="data/callbox_example.jpg" width="350" height="500">
</p>

## Process

In order to better understand the business problem, we contacted the McGill Security team who graciously gave us all the detailed necessary information. We obtained costs for installing and maintaining the different types of callboxes as well gathered as information on the priority locations for these boxes. In particular we used the McGill night route map to generate a set of demand points to be covered. From there we brainstormed a mathematical formulation for the problem and coded out the formulation in Gurobi.

### Night Route Map
[View Full Route Map (PDF)](data/campus_map.pdf)

## Results

The model achieved a **61.2% demand point coverage** for **$251,000 CAD**, installing 15 new phones and replacing six old phones. One important note here is that due to the construction of the night route map it is impossible to cover more than 75% of all demand points. Overall, this gave the security team a clear capital cost for an emergency callbox overhaul and could be weighed up against other competing upgrades/improvements in their budget meetings. Another recommendation as a result of this project was to alter the night route away from streets (such as Park Ave) which lack McGill buildings, and therefore options to install callboxes on, and instead keep the route going by more McGill buildings such as Durocher.

![Results](data/callbox_results.png)

## Team

Rui Zhao, Serena Sun, Arantzazu Arregui Gonzalez, Chloee Liew, Nicholas Stanfield
