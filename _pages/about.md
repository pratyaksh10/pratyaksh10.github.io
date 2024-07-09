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
    2024 IEEE/RSJ International Conference on Intelligent Robots and Systems, Abu Dhabi (Accepted) <br>
    [[paper](https://arxiv.org/pdf/2211.16988)]<br>
    <details>
    <span style="font-size: 14px">Accurate modeling of system dynamics is crucial for achieving high-performance planning and control of robotic systems. Although existing data-driven approaches represent a promising approach for modeling dynamics, their accuracy is limited to a short prediction horizon, overlooking the impact of compounding prediction errors over longer prediction horizons. Strategies to mitigate these cumulative errors remain underexplored. To bridge this gap, in this paper, we study the key design choices for efficiently learning long-horizon prediction dynamics for quadrotors. Specifically, we analyze the impact of multiple architectures, historical  data, and multi-step loss formulation. We show that sequential modeling techniques showcase their advantage in minimizing compounding errors compared to other types of solutions. Furthermore, we propose a novel decoupled dynamics learning approach, which further simplifies the learning process while also enhancing the approach modularity.Extensive experiments and ablation studies on real-world quadrotor data demonstrate the versatility and precision of the proposed approach. Our outcomes offer several insights and methodologies for enhancing long-term predictive accuracy of learned quadrotor dynamics for planning and control.</span>
    </details>
    </td>
</tr>


<tr>
<td markdown="span" style="text-align: center;vertical-align: middle;border-left-style: none;border-right-style: none;"><img src="{{ site.baseurl }}/images/TO-DO.png"></td>
<td markdown="span" style="vertical-align: middle;border-left-style: none;border-right-style: none;">
    **QuadFormer: Real-Time Unsupervised Power Line Segmentation with Transformer-Based Domain Adaptation**<br>
    **Pratyaksh Prabhav Rao**<sup>*</sup>, Feng Qiao<sup>*</sup>, Weide Zhang, Yiliang Xu, Yong Deng, Guangbin Wu, Qiang Zhang, and Giuseppe Loianno.<br>
    21st International Conference on Ubiquitous Robots (UR), New York (Accepted) <br>
    [[paper]()] [[video](https://www.youtube.com/watch?v=7h-lqGbQCSg)]<br>
    <details>
    <span style="font-size: 14px">Accurately identifying Power Lines (PLs) is crucial for ensuring the safety of aerial vehicles. Despite the potential of recent deep learning approaches, obtaining high-quality ground truth annotations remains a challenging and labor-intensive task. Unsupervised Domain Adaptation (UDA) emerges as a promising solution, leveraging knowledge from labeled synthetic data to improve performance on unlabeled real images. However, existing UDA methods often suffer of huge computation costs, limiting their deployment on real-time embedded systems commonly utilized on aerial vehicles. To mitigate this problem, this paper introduces QuadFormer, a real-time framework designed for unsupervised semantic segmentation within the UDA paradigm. QuadFormer integrates a lightweight transformer-based segmentation model with a cross-attention mechanism to narrow the gap between a labelled synthetic domain and unlabelled real domain. Furthermore, we design a novel pseudo label scheme to enhance the segmentation accuracy of the unlabelled real data. To facilitate the evaluation of our framework and promote reserach in PL segemntation, we present two new datasets: AutelPL Synthetic and AutelPL Real. Experimental results demonstrate that QuadFormer achieves state-of-the-art performance on both AutelPL Synthetic to TTPLA and AutelPL Synthetic to AutelPL Real tasks. We will publicly release the dataset to the research community.</span>
    </details>
    </td>
</tr>

<tr>
<td markdown="span" style="text-align: center;vertical-align: middle;border-left-style: none;border-right-style: none;"><img src="{{ site.baseurl }}/images/TO-DO.png"></td>
<td markdown="span" style="vertical-align: middle;border-left-style: none;border-right-style: none;">
    **Unifying Foundation Models with Quadrotor Control for Visual Tracking Beyond Object Categories**<br>
    Alessandro Saviolo<sup>*</sup>, **Pratyaksh Rao**<sup>*</sup>, Vivek Radhakrishnan, Jiuhong Xiao, and Giuseppe Loianno.<br>
    2024 IEEE International Conference on Robotics and Automation, Yokohama <br>
    [[paper](https://arxiv.org/pdf/2310.04781)] [[video](https://www.youtube.com/watch?v=35sX9C1wUpA)]<br>
    <details>
    <span style="font-size: 14px">Visual control enables quadrotors to adaptively navigate using real-time sensory data, bridging perception with action. Yet, challenges persist, including generalization across scenarios, maintaining reliability, and ensuring real-time responsiveness. This paper introduces a perception framework grounded in foundation models for universal object detection and tracking, moving beyond specific training categories. Integral to our approach is a multi-layered tracker integrated with the foundation detector, ensuring continuous target visibility, even when faced with motion blur, abrupt light shifts, and occlusions. Complementing this, we introduce a model-free controller tailored for resilient quadrotor visual tracking. Our system operates efficiently on limited hardware, relying solely on an onboard camera and an inertial measurement unit. Through extensive validation in diverse challenging indoor and outdoor environments, we demonstrate our system’s effectiveness and adaptability. In conclusion, our research represents a step forward in quadrotor visual tracking, moving from taskspecific methods to more versatile and adaptable operations.</span>
    </details>
    </td>
</tr>

<tr>
<td markdown="span" style="text-align: center;vertical-align: middle;border-left-style: none;border-right-style: none;"><img src="{{ site.baseurl }}/images/TO-DO.png"></td>
<td markdown="span" style="vertical-align: middle;border-left-style: none;border-right-style: none;">
    **Learning to Listen and Move: An Implementation of Audio-Aware Mobile Robot Navigation in Complex Indoor Environment**<br>
    Pratyaksh P. Rao and Abhra Roy Chowdhury.<br>
    2022 IEEE International Conference on Robotics and Automation, Philadelphia <br>
    [[paper](https://ieeexplore.ieee.org/abstract/document/9812193)] [[video](https://www.youtube.com/watch?v=xM2LUYEGRRs&t=1s)]<br>
    <details>
    <span style="font-size: 14px">Sound is an essential navigation cue that intelligent robots can leverage for localizing sound-emitting targets. This work introduces a framework for the audio-aware navigation task of mobile robots equipped with a microphone array in a complex indoor environment. The robot initialized at a random starting position has to accurately localize a distant sound source and plan an optimal path towards the sound-emitting target. Auto-encoders are used to extract implicit acoustic features that are robust against environmental noise and reverberation. The proposed framework is based on two key ideas - a sound inference module (SIM) that maps the perceived acoustic information to a given geometric map of the physical space, and a path planner that generates a path from the robot's current position to the estimated position of the sound source. Experimental results show that the SIM achieved a minimum and maximum localization error of 0.31 m and 0.70 m at a robot-source distance of 1 m and 6 m, respectively at different environmental configurations. Additionally, the proposed framework achieved a minimum and maximum reliability of 4.38 m^1 and 2.31 m^1 at a robot-source distance of 1 m and 6 m, respectively under the influence of background noise.</span>
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