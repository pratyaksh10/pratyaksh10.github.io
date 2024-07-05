---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I’m an incoming PhD student at the [Agile Robotics and Perception Lab (ARPL)](https://wp.nyu.edu/arpl/), New York University. My research interests pertain to developing algorithms to facilitate autonomous navigation of aerial vehicles, particularily in the wild. I obtained my M.S. degree from New York University and B.S. degree from Manipal Institute of Technology.

<style>
    .toggle-container {
        cursor: pointer;
        display: flex;
        align-items: center;
        font-size: 22px; /* Larger font size */
        color: #007bff; /* Blue color */
        font-weight: bold; /* Bold text */
    }

    .triangle {
        width: 0;
        height: 0;
        border-top: 6px solid transparent;
        border-bottom: 6px solid transparent;
        border-left: 10px solid black; /* Pointing to the right */
        margin-right: 8px;
        transition: transform 0.3s;
    }

    .triangle.open {
        transform: rotate(90deg);
    }

    .news-content {
        display: block;
        margin-top: 10px;
        overflow: hidden;
        max-height: 24px; /* Limit the max height to show only 2 items initially */
        transition: max-height 0.3s ease-out;
    }

    .news-content.open {
        max-height: none; /* Expand to show all items when open */
    }
</style>

<div class="toggle-container" onclick="toggleNews()">
    <div class="triangle" id="triangle"></div>
    <span>News!</span>
</div>



<div id="news" class="news-content">
    <!-- Your news content goes here -->
    <li>Jul 2024, paper accepted by the 2024 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS 2024), Abu Dabi.</li>
    <!-- <ul> -->
    <li>Received best M.S. Thesis Award at the NYU 2024 Commencement Awards Ceremony</li>
    <li>Apr 2024, our work <a href="https://arxiv.org/abs/2211.16988">QuadFormer</a> was accepted by the 21st International Conference on Ubiquitous Robots (UR), New York.</li>
    <li>Jan 2024, our work <a href="https://arxiv.org/pdf/2310.04781">Unifying Foundation Models with Quadrotor Control for Visual Tracking Beyond Object Categories</a> was accepted by the  IEEE International Conference on
Robotics and Automation (ICRA), Yokohama.</li>
    <!-- </ul> -->
</div>

<script>
    function toggleNews() {
        var newsDiv = document.getElementById("news");
        var triangle = document.getElementById("triangle");
        if (newsDiv.classList.contains("open")) {
            newsDiv.classList.remove("open");
            triangle.classList.remove("open");
        } else {
            newsDiv.classList.add("open");
            triangle.classList.add("open");
        }
    }
</script>

## Research & Publications
<table frame=hsides style="border-left-style: none;border-right-style: none;">
<colgroup>
<col width="30%" />
<col width="70%" />
</colgroup>
<thead>
</thead>
<tbody>

<tr>
<td markdown="span" style="text-align: center;vertical-align: middle;border-left-style: none;border-right-style: none;"><img src="{{ site.baseurl }}/images/TO-DO.png"></td>
<td markdown="span" style="vertical-align: middle;border-left-style: none;border-right-style: none;">
    **Learning Long-Horizon Predictions for Quadrotor Dynamics**<br>
    **Pratyaksh Prabhav Rao**, Alessandro Saviolo, Tommaso Castiglione Ferrari, and Giuseppe Loianno.<br>
    <!-- European Conference on Computer Vision (ECCV), 2024 in submission<br> -->
    <!-- [[paper](https://arxiv.org/abs/2310.08820v2)]<br> -->
    <details>
    <span style="font-size: 14px">Accurate modeling of system dynamics is crucial for achieving high-performance planning and control of robotic systems. Although existing data-driven approaches represent a promising approach for modeling dynamics, their accuracy is limited to a short prediction horizon, overlooking the impact of compounding prediction errors over longer prediction horizons. Strategies to mitigate these cumulative errors remain underexplored. To bridge this gap, in this paper, we study the key design choices for efficiently learning long-horizon prediction dynamics for quadrotors. Specifically, we analyze the impact of multiple architectures, historical  data, and multi-step loss formulation. We show that sequential modeling techniques showcase their advantage in minimizing compounding errors compared to other types of solutions. Furthermore, we propose a novel decoupled dynamics learning approach, which further simplifies the learning process while also enhancing the approach modularity.Extensive experiments and ablation studies on real-world quadrotor data demonstrate the versatility and precision of the proposed approach. Our outcomes offer several insights and methodologies for enhancing long-term predictive accuracy of learned quadrotor dynamics for planning and control.</span>
    </details>
    </td>
</tr>


</tbody>
</table>


## Honors and Awards

<div class="honors-awards">
    <ul>
        <li>Received best M.S. Thesis Award at the NYU 2024 Commencement Awards Ceremony.</li>
        <li>Presented a Technical Research Paper at the 21st International Conference on Ubiquitous Robots (UR), New York, USA.</li>
        <li>Presented a Technical Research Paper at the 2022 IEEE International Conference on Robotics and Automation (ICRA), 2022, Philadelphia, USA.</li>
        <li>Presented a Technical Research Poster at the 2021 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS) (IROS 2021),Prague, Czech Republic</li>
        <li> Best project award at the Experts Hub Innovation Challenge 2019, Chennai, India.</li>
    </ul>
</div>
<!-- 
## Activities

<div class="activities">
    <ul>
        <li>Presented a Technical Research Paper at the 21st International Conference on Ubiquitous Robots (UR), New York, USA.</li>
        <li>Presented a Technical Research Paper at the 2022 IEEE International Conference on Robotics and Automation (ICRA), 2022, Philadelphia, USA.</li>
        <li>Presented a Technical Research Poster at the 2021 IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS) (IROS 2021),Prague, Czech Republic</li>
        <li> Best project award at the Experts Hub Innovation Challenge 2019, Chennai, India.
    </ul>
</div> -->

<!-- <script type="text/javascript" id="clustrmaps" src="//clustrmaps.com/map_v2.js?d=shW72uw30kk16-iNF-9p2HCZ7qJI1k9hYDoMXjyKpHU&cl=ffffff&w=a"></script> -->