---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<script src="Home/assets/js/abstract-toggle.js"></script>


<span class='anchor' id='about-me'></span>
# <span style="font-weight: bold; color: #654f4fcb; font-size: 28px;">⭐ Short Bio</span>
<p style="font-family: Arial, sans-serif;">
    Hello! I am Yichen Luo, a Ph.D. student in Computer Science at 
    <a href="https://www.wm.edu/" target="_blank" style="color: #35705D; text-decoration: underline;">William & Mary</a>, 
    under the mentorship of 
    <a href="https://sidilu.org/" target="_blank" style="color: #35705D; text-decoration: underline;">Dr. Sidi Lu</a>. 
    I earned my B.E. degree from Shanghai Dianji University in 2023. My research interests span the <em> Internet of Things, 
    autonomous driving, sensor systems, edge intelligence, and vehicle computing </em>. I focus on designing innovative solutions 
    for connected and intelligent vehicles, leveraging cutting-edge technologies to enhance performance and safety.
</p>

<div><hr style="border: 0; border-top: 1px solid #dcdcdc; margin: 10px 0;"></div>


<br>
<span class='anchor' id='news'></span>
# <span style="font-weight: bold; color: #654f4fcb; font-size: 28px;">🔥 News</span>
<p style="font-family: Arial, sans-serif;">- 2024: NSF ACM/IEEE Symposium on Edge Computing (SEC) Student Travel Grant. &nbsp;🎉 </p>
<p style="font-family: Arial, sans-serif;">- 2024: International Student Opportunity Scholarship at William & Mary. &nbsp;🎉</p>
<div><hr style="border: 0; border-top: 1px solid #dcdcdc; margin: 10px 0;"></div>


<br>
<span class='anchor' id='publications'></span>
# <span style="font-weight: bold; color: #654f4fcb; font-size: 28px;">📜 Publications </span>


<div class="paper-list"> 
   <!-- 2024-->
  <div class="paper-item">
    <!-- Date -->
    <div class="date"> 
      <h5>2024</h5>
    </div>
    <!-- Paper details -->
    <div class="pap">
      <a href="./pdf/SEC24-VEC.pdf">An Efficient Data Transmission Framework for Connected Vehicles</a> <br>
      <p style="margin-left: 6px; font-family: Arial, sans-serif; font-size: 16px; font-weight: normal;">
        <b>Yichen Luo</b>, Yongtao Yao, Junzhou Chen, Sidi Lu, and Weisong Shi.<br>
        The 9th ACM/IEEE Symposium on Edge Computing (SEC), Rome, Italy.
      </p>
      <p style="margin-left: 4px; font-weight: normal; margin-top: -5px;">
        <!-- Abstract toggle button -->
        <a href="#" id="abstract-button-sec24" onclick="toggleAbstract('abstract-sec24'); return false;" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px; cursor: pointer;">[Abstract]</a>
        <a href="./pdf/SEC24-VEC.pdf" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[PDF] </a>
        <a href="https://drive.google.com/file/d/17voEyOaxGxl2kotKK8oH6yGPm6_HoXTP/view?usp=sharing" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[Video] </a>
        <a href="https://drive.google.com/file/d/1aquo75jCKTwzXN7moM1T5BfhhcfT3Kh_/view?usp=sharing" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[Poster] </a>
        <a href="https://acm-ieee-sec.org/2024/" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[Conference] </a> 
      </p>
      <!-- Abstract content (hidden by default) -->
      <div id="abstract-sec24" style="display: none; margin-top: 10px; font-family: Arial, sans-serif; font-size: 14px; font-weight: normal; border-left: 4px solid #165740; padding-left: 10px;">
        Connected vehicles (CVs) face challenges in continuous big data transmission, resulting in high transmission bandwidth costs and impacting real-time decision-making. To address this, we propose two dynamic, driving-aware compression mechanisms based on reinforcement learning and temporal compressive sensing to intelligently compress video data. These mechanisms adapt to driving conditions, reducing bandwidth while preserving sufficient information for accurate applications such as object detection and ensuring high-quality reconstruction when needed. We also implement a Vehicle-EdgeServer-Cloud (VEC) closed-loop framework that integrates these mechanisms. Specifically, a lightweight vehicle model performs real-time detection on compressed data (measurements), while the EdgeServer receives measurements and reconstructs scenes if needed. The measurements, reconstructed video, and analysis results are then sent to the cloud for vehicle model updates. Unlike conventional methods, our framework seamlessly adapts across vehicles, EdgeServers, and the cloud, supporting efficient data transmission and dynamic model updates. Extensive evaluations were conducted on our designed roadside unit platform and robotic vehicle, both equipped with industry-grade sensors and computing units. The results demonstrate an 18× reduction in bandwidth at 320KB/s while maintaining high detection accuracy and reconstruction quality compared to non-adaptive measurements, highlighting the framework's promising real-world applications for CVs.
      </div>
    </div>
  </div>


<script>
  // Function to toggle abstract visibility
  function toggleAbstract(id) {
    var abstract = document.getElementById(id);
    if (abstract.style.display === "none") {
      abstract.style.display = "block";
    } else {
      abstract.style.display = "none";
    }
  }

  // Global click listener to hide abstract if clicked outside
  document.addEventListener("click", function (event) {
    // Abstract elements and their corresponding buttons
    var abstract = document.getElementById("abstract-sec24");
    var button = document.getElementById("abstract-button-sec24");

    // Check if the click is outside both the abstract and the button
    if (
      abstract.style.display === "block" &&
      !abstract.contains(event.target) &&
      !button.contains(event.target)
    ) {
      abstract.style.display = "none";
    }
  });

  // Prevent click event on button from propagating to the document
  document.getElementById("abstract-button-sec24").addEventListener("click", function (event) {
    event.stopPropagation(); // Prevents event bubbling
  });

  // Prevent click event on abstract content from propagating to the document
  document.getElementById("abstract-sec24").addEventListener("click", function (event) {
    event.stopPropagation(); // Prevents event bubbling
  });
</script>

  
<!-- IOTJ-realtime -->
<div class="paper-item">
  <div class="date">
    <h5></h5>
  </div>
  <div class="pap">
    <!-- Paper title -->
    <a href="./pdf/IOTJ_24_Towards_Real-Time.pdf">Towards Real-Time and Efficient Perception Workflows in Software-Defined Vehicles</a> <br>
    <p style="margin-left: 6px; font-family: Arial, sans-serif; font-size: 16px; font-weight: normal;">
      Sumaiya, Reza Jafarpourmarzouni, <b>Yichen Luo</b>, Sidi Lu, and Zheng Dong.<br>
      IEEE Internet of Things Journal.
    </p>
    <p style="margin-left: 4px; font-weight: normal; margin-top: -5px;">
      <!-- Abstract toggle button -->
      <a href="#" id="abstract-button-iotj" onclick="toggleAbstract('abstract-iotj'); return false;" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px; cursor: pointer;">[Abstract]</a>
      <a href="./pdf/IOTJ_24_Towards_Real-Time.pdf" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[PDF]</a>
      <a href="https://ieee-iotj.org/" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[Conference]</a>
    </p>
    <!-- Abstract content (hidden by default) -->
    <div id="abstract-iotj" style="display: none; margin-top: 10px; font-family: Arial, sans-serif; font-size: 14px; font-weight: normal; border-left: 4px solid #165740; padding-left: 10px;">
      With the growing demand for software-defined vehicles (SDVs), deep learning-based perception models have become increasingly important in intelligent transportation systems. However, these models face significant challenges in enabling real-time and efficient SDV solutions due to their substantial computational requirements, often unavailable in resource-constrained vehicles. As a result, these models typically suffer from low throughput, high latency, and excessive GPU/memory usage, making them impractical for real-time SDV applications. To address these challenges, our research focuses on optimizing model and workflow performance by integrating pruning and quantization techniques across various computational environments, utilizing frameworks such as PyTorch, ONNX, ONNX Runtime, and TensorRT. We systematically explore and evaluate three distinct pruning methods in combination with multi-precision quantization workflows (FP32, FP16, and INT8) and present the results based on four evaluation metrics: inference throughput, latency, GPU/memory usage, and accuracy. Our designed techniques, including pruning and quantization, along with optimized workflows, can achieve up to 18$\times$ faster inference speed and 16.5$\times$ higher throughput, while reducing GPU/memory usage by up to 30%, all with minimal impact on accuracy. Our work suggests using the Torch-ONNX-TensorRT workflow quantized with FP16 precision and group pruning as the optimal strategy for maximizing inference performance. It demonstrates great potential in optimizing real-time, efficient perception workflows in SDVs, contributing to the enhanced application of deep learning models in resource-constrained environments.
    </div>
  </div>
</div>

<script>
  // Function to toggle abstract visibility
  function toggleAbstract(id) {
    var abstract = document.getElementById(id);
    if (abstract.style.display === "none") {
      abstract.style.display = "block";
    } else {
      abstract.style.display = "none";
    }
  }

  // Global click listener to hide abstract if clicked outside
  document.addEventListener("click", function (event) {
    // Abstract elements and their corresponding buttons
    var abstract = document.getElementById("abstract-iotj");
    var button = document.getElementById("abstract-button-iotj");

    // Check if the click is outside both the abstract and the button
    if (
      abstract.style.display === "block" &&
      !abstract.contains(event.target) &&
      !button.contains(event.target)
    ) {
      abstract.style.display = "none";
    }
  });

  // Prevent click event on button from propagating to the document
  document.getElementById("abstract-button-iotj").addEventListener("click", function (event) {
    event.stopPropagation(); // Prevents event bubbling
  });

  // Prevent click event on abstract content from propagating to the document
  document.getElementById("abstract-iotj").addEventListener("click", function (event) {
    event.stopPropagation(); // Prevents event bubbling
  });
</script>



  
<!-- MOST-raindrop -->
<div class="paper-item">
  <div class="date">
    <h5></h5>
  </div>
  <div class="pap">
    <!-- Paper title -->
    <a href="./pdf/MOST24-Raindrop.pdf">Impact of Raindrops on Camera-Based Detection in Software-Defined Vehicles</a> <br>
    <p style="margin-left: 6px; font-family: Arial, sans-serif; font-size: 16px; font-weight: normal;">
      <b>Yichen Luo</b>, Daoxuan Xu, Gang Zhou, Yifan Sun, and Sidi Lu.<br>
      IEEE International Conference on Mobility, Operations, Services, and Technologies (MOST), Dallas, TX.
    </p>
    <p style="margin-left: 4px; font-weight: normal; margin-top: -5px;">
      <!-- Abstract toggle button -->
      <a href="#" id="abstract-button-raindrop" onclick="toggleAbstract('abstract-raindrop'); return false;" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px; cursor: pointer;">[Abstract]</a>
      <a href="./pdf/MOST24-Raindrop.pdf" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[PDF]</a>
      <a href="https://drive.google.com/file/d/1yBGxDYc8-d9_UiVdmmfR_kt42lkxN1K6/view?usp=sharing" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[Poster]</a>
      <a href="https://ieeemobility.org/MOST2024/" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[Conference]</a>
    </p>
    <!-- Abstract content (hidden by default) -->
    <div id="abstract-raindrop" style="display: none; margin-top: 10px; font-family: Arial, sans-serif; font-size: 14px; font-weight: normal; border-left: 4px solid #165740; padding-left: 10px;">
      Raindrops adhering to windshields or camera lenses substantially impair visibility, leading to significant camera-based detection challenges for software-defined vehicles in both daytime and nighttime conditions. Addressing the impact of raindrops is thus crucial. This work begins by classifying four prevalent types of raindrops within the BDD100K dataset, identifying microsphere raindrops as particularly impactful in rainy conditions. We then conduct a quantitative analysis focusing on the density and diameter of raindrops, underscoring the pronounced impacts of small-density raindrops on detection performance. To mitigate raindrop interference, we introduce and assess the SR3 model for raindrop removal, applying it to both synthetic raindrop-degraded data and real-world rainy data. Besides, we propose YOLO-RA, a novel and fast model to resolve the issues of missing small-size objects and erroneous detections in irrelevant regions. Next, a novel pipeline that combines SR3 with YOLO-RA markedly improves accuracy and processing speed. Finally, we discuss our experimental observations extensively and offer detailed explanations, contributing to understanding SDVs' operational effectiveness in adverse weather conditions.
    </div>
  </div>
</div>

<script>
  // Function to toggle abstract visibility
  function toggleAbstract(id) {
    var abstract = document.getElementById(id);
    if (abstract.style.display === "none") {
      abstract.style.display = "block";
    } else {
      abstract.style.display = "none";
    }
  }

  // Global click listener to hide abstract if clicked outside
  document.addEventListener("click", function (event) {
    // Abstract elements and their corresponding buttons
    var abstract = document.getElementById("abstract-raindrop");
    var button = document.getElementById("abstract-button-raindrop");

    // Check if the click is outside both the abstract and the button
    if (
      abstract.style.display === "block" &&
      !abstract.contains(event.target) &&
      !button.contains(event.target)
    ) {
      abstract.style.display = "none";
    }
  });

  // Prevent click event on button from propagating to the document
  document.getElementById("abstract-button-raindrop").addEventListener("click", function (event) {
    event.stopPropagation(); // Prevents event bubbling
  });

  // Prevent click event on abstract content from propagating to the document
  document.getElementById("abstract-raindrop").addEventListener("click", function (event) {
    event.stopPropagation(); // Prevents event bubbling
  });
</script>

  <!-- 2023-->
  <div class="paper-item">
    <!-- Data -->
      <div class="date"> <h5>2023</h5></div>
      <!-- EAI-Battery -->
      <div class="pap">
        <a href="https://link.springer.com/content/pdf/10.1007/978-3-031-53401-0_19.pdf">Improved Solar Photovoltaic Panel Defect  Detection Technology Based on YOLOv5</a> <br>
        <p style="margin-left: 6px; font-family: Arial, sans-serif; font-size: 16px; font-weight: normal;">
          Shangxian Teng, Zhonghua Liu, <b>Yichen Luo</b>, and Pengpeng Zhang.<br>
          The 6th EAI International Conference on 6G for Future Wireless Networks, Shanghai, China.</p>
        <p style="margin-left: 4px; font-weight: normal; margin-top: -5px;">
          <a href="https://link.springer.com/content/pdf/10.1007/978-3-031-53401-0_19.pdf" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[PDF] </a>
          <a href="https://5gwn.eai-conferences.org/2023/" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[Conference] </a> 
        </p>
      </div>
  </div>
      <!-- EAI-Plastic Runway-->
  <div class="paper-item">
    <div class="date"> <h5></h5></div>
      <div class="pap">
        <a href="https://link.springer.com/content/pdf/10.1007/978-3-031-53404-1_12.pdf">Multiple Color Feature and Contextual Attention Mechanism Based on YOLOX </a> <br>
        <p style="margin-left: 6px; font-family: Arial, sans-serif; font-size: 16px; font-weight: normal;">
          Shuaidi Shan, Pengpeng Zhang, Xinlei Wang, Shangxian Teng, and <b>Yichen Luo</b>.<br>
          The 6th EAI International Conference on 6G for Future Wireless Networks, Shanghai, China.</p>
        <p style="margin-left: 4px; font-weight: normal; margin-top: -5px;">
          <a href="https://link.springer.com/content/pdf/10.1007/978-3-031-53404-1_12.pdf" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[PDF] </a>
          <a href="https://5gwn.eai-conferences.org/2023/" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">[Conference] </a> 
        </p>
      </div>
  </div>

</div>

<div><hr style="border: 0; border-top: 1px solid #dcdcdc; margin: 10px 0;"></div>



<br>
<span class='anchor' id='research-project'></span>
# <span style="font-weight: bold; color: #654f4fcb; font-size: 28px;">📚 Research Project</span>

<h2 style="font-size: 24px; font-family: Arial, sans-serif;">🕰️ PhD Journey</h2>

<!-- OTA-->
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Currently</div><img src='proj_img/OTA-draft.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<div class="paper-item"> <a href="#" style="margin-left: -5px;">Incremental over-the-air (OTA) updates for software-defined vehicles</a> </div>

<em>My role: Project Leader</em>
- Propose a software OTA update framework for software-defined vehicles (SDVs), leveraging a robotic vehicle and an industry-grade roadside unit (RSU)
- Develop RSU- and vehicle-side mechanisms to support incremental updates, enhancing efficiency in software version management
- Assess the performance of Cellular Vehicle-to-Everything (C-V2X) technology, combining V2X and 5G, along with Wi-Fi communication for efficient OTA transmission.
</div>
</div>


<!-- SEC-VEC-->
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">2024 Spring</div><img src='proj_img/SEC-hardware.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<div class="paper-item"> <a href="pdf/SEC24-VEC.pdf" style="margin-left: -5px;">An Efficient Data Transmission Framework for Connected Vehicles</a> </div>

<em>My role: Project Leader</em>
- <span style="text-decoration: underline; text-decoration-thickness: 2px;">
  Two Reinforcement Learning (RL) Policies:</span> We design two vehicle-based RL policies (tracking-driven and similarity-driven) to dynamically TCS vehicles based on real-time driving conditions.
- <span style="text-decoration: underline; text-decoration-thickness: 2px;"> Vehicle-EdgeServer-Cloud (VEC) Framework:</span> This framework integrates adaptive compression mechanisms to streamline information flow: vehicles perform real-time object detection on compressed data, EdgeServers reconstruct scenes as needed, and the cloud aggregates results for continuous model updates across the network.
</div>
</div>

<!-- MOST-Raindrop-->
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">2023 Fall</div><img src='proj_img/rain_frame.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<div class="paper-item"> <a href="pdf/MOST24-Raindrop.pdf" style="margin-left: -5px;">Impact of Raindrops on Camera-Based Detection in Software-Defined Vehicles</a> </div>

<em>My role: Project Leader</em>
- Conduct a comprehensive qualitative analysis of raindrops during daytime and nighttime.
- Design a quantitative analysis to assess the diverse influences of raindrops.
- Develop and propose two innovative methods to effectively eliminate the detrimental influence of raindrops, enhancing the robustness and reliability of the system.
</div>
</div>

<!-- DEMO in PhD -->
<h2 style="font-size: 20px; font-family: Arial, sans-serif;">🎥 DEMO</h2>
<div class="paper-box" style="position: relative; top: -20px;">
  <div class="gif-container" style="position: relative; top: -10px; display: flex; justify-content: space-between; align-items: flex-start;">
    <!-- image and Description -->
    <div class="gif-item" style="flex: 1; text-align: center;">
      <div class="label" style="color: #fff; font-size: 12px; margin-bottom: 10px; background-color: #165740; padding: 5px 10px; display: inline-block;">Simulation</div>
      <img src="proj_img/CARLA_manu.gif" alt="GIF 1" style="width: auto; height: 170px; object-fit: cover;">
      <div>
        <p style="margin-top: 5px; font-size: 12px;">Manual control in CARLA.</p>
      </div> 
    </div>
    <div class="gif-item" style="flex: 1; text-align: center;">
      <div class="label" style="color: #fff; font-size: 12px; margin-bottom: 10px; background-color: #165740; padding: 5px 10px; display: inline-block;">Robotic Vehicle</div>
      <img src="proj_img/ROS_Vehicle.gif" alt="GIF 2" style="width: auto; height: 170px; object-fit: cover;">
      <div>
        <p style="margin-top: 5px; font-size: 12px;">Robotic vehicle on the track map.</p>
      </div>
    </div>
    <div class="gif-item" style="flex: 1; text-align: center;">
      <div class="label" style="color: #fff; font-size: 12px; margin-bottom: 10px; background-color: #165740; padding: 5px 10px; display: inline-block;">Robotic Vehicle</div>
      <img src="proj_img/robot_detect.gif" alt="GIF 3" style="width: auto; height: 170px; object-fit: cover;">
      <div>
        <p style="margin-top: 5px; font-size: 12px;">Visual data captured by the robotic vehicle.</p>
      </div>
    </div>
  </div>
</div>



<h2 style="font-size: 24px; font-family: Arial, sans-serif;">🌱 Undergraduate Journey</h2>


<!-- Lit-->
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">2023 Summar</div><img src='proj_img/Lit.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<div class="paper-item"> <a href="https://kororinpas.github.io/talks/programme_3" style="margin-left: -5px;">Lit-Cite</a> </div>
<span>Manager: <a href="https://kororinpas.github.io/" target="_blank" style="color: #35705D; text-decoration: underline;">Zekai Shen</a></span><br>
<em>My role: Project Member</em>
- Lit_Cite is an AI-driven software tool utilizing Retriever-Augmented Generation (RAG) technology to streamline the citation process for researchers.
- Users upload a PDF to create a library of potential citations, with the software extracting key information. Highlighted sentences are matched to relevant citations using a word vector algorithm, which is then automatically added.
- The program won a Third Prize in China's First National Large Language Model Innovation and Creative Application Competition. 
    <a href="https://kororinpas.github.io/awards/award-1/" target="_blank" style="text-decoration: none; font-family: Arial, sans-serif; font-size: 14px;">🏆 [Award] </a>
</div>
</div>

<!-- Plastic Runway-->
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">2022 Fall - 2023 Spring</div><img src='proj_img/plastic-sys.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">
<div class="paper-item"> <a href="https://link.springer.com/content/pdf/10.1007/978-3-031-53404-1_12.pdf" style="margin-left: -5px;">Plastic Runway Surface Damage Detection System</a> </div>
<em>Team: Shuaidi Shan, Xinlei Wang, Yichen Luo</em><br>
<em>My role: Project Leader</em>
- Utilize Raspberry Pi 3B+ and a vehicle-mounted video camera for collecting picture information; also employ Wi-Fi, TCP Protocol, and Secure Shell (SSH) for communication between the upper computer and the lower computer.
- For the front-end and back-end, I build the web page with Django and enable the picture uploading function through POST requests. The customer runs YOLOX to conduct tests and receives output from the client. I also create the database with MySQL to support the front-end.
- Modify underlying algorithms by adopting traditional computer vision and pruning methods to improve recognition accuracy and speed.
</div>
</div>


<!-- Greenhouse -->
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">2020 Fall - 2021 Spring</div><img src='proj_img/Greenhouse.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<div class="paper-item"> <a href="#" style="margin-left: -5px;">IoT Technology in Agriculture: Designing an Intelligent Greenhouse</a> </div>
<em>Team: Maoxuan Yao, Yichen Luo</em>
- Utilizing LoRa (Long Range) technology for wireless communication between sensors ensures lower power consumption. Development with TPYboardv102 includes configuring vital parameters such as temperature, moisture, and illumination intensity to enable real-time monitoring and transmission in the greenhouse.
- Collaborating on the greenhouse model involves setting up various equipment for performance testing in labs. Conducting field surveys of nearby farms provides inspiration for designing a more intelligent and energy-efficient system.
- Learning and documenting demand analyses and product descriptions for embedded temperature controllers involve drawing flowcharts. Adopting Unified Modeling Language (UML) enhances the description of system commands written in Python, improving user comprehension.
</div>
</div>


<!-- DEMO -->
<h2 style="font-size: 20px; font-family: Arial, sans-serif;">🎥 DEMO</h2>
<div class="paper-box" style="position: relative; top: -20px;">
  <div class="gif-container" style="position: relative; top: -10px;">
    <!-- 图片和文字说明 -->
    <div class="gif-item">
      <div class="label" style="color: #fff; font-size: 12px; margin-bottom: 10px; background-color: #165740; padding: 5px 10px; display: inline-block;">Greenhouse</div>
      <img src="proj_img/GreenHouse.gif" alt="GIF 1">
      <div>
        <p style="position: relative; top: 5px; font-size: 12px;">Laboratory Environment</p>
      </div> 
    </div>
    <div class="gif-item">
      <div class="label" style="color: #fff; font-size: 12px; margin-bottom: 10px; background-color: #165740; padding: 5px 10px; display: inline-block;">Line-Following Robot Car</div>
      <img src="proj_img/car.gif" alt="GIF 2">
      <div>
        <p style="position: relative; top: 5px; font-size: 12px;">
        The vehicle leverages infrared sensors to analyze and interpret the path
        </p>
      </div>
    </div>
  </div>
</div>

<span class='anchor' id='internships'></span>
# <span style="font-weight: bold; color: #654f4fcb; font-size: 28px;">💻 Internships </span>
  <div style="font-family: Arial, sans-serif; line-height: 1.6; margin: 12px;">
        <div style="margin-bottom: 10px; display: flex; justify-content: space-between; align-items: center; font-size: 16px;">
            <span>
                2024.07 - 2024.08, 
                <a href="https://www.thecarlab.org/" target="_blank" style="color: #35705D; text-decoration: underline;">The CAR Lab</a>, Newark, DE, USA
            </span>
            <span>Research Intern | The CAR Lab</span>
        </div>
        <div style="margin-bottom: 10px; display: flex; justify-content: space-between; align-items: center; font-size: 16px;">
            <span>Mentor: <a href="https://www.weisongshi.org/" target="_blank" style="color: #35705D; text-decoration: underline;">Weisong Shi</a></span>
        </div>
        <div style="font-size: 14px;">
            <em>My role</em>: Develop a software over-the-air (OTA) update framework for heterogeneous software-defined vehicles (SDVs), leveraging a robotic vehicle and an industry-grade roadside unit (RSU) for efficient deployment and management.
        </div>
    </div>
<div><hr style="border: 0; border-top: 1px solid #dcdcdc; margin: 10px 0;"></div>


  <div style="font-family: Arial, sans-serif; line-height: 1.6; margin: 12px;">
        <div style="margin-bottom: 10px; display: flex; justify-content: space-between; align-items: center; font-size: 16px;">
            <span>
                2022.06 - 2022.11, 
              <a href="https://www.bayer.com.cn/en/" target="_blank" style="color: #35705D; text-decoration: underline;">Bayer Consumer Health</a>, SH, CN
            </span>
            <span>Algorithm Engineer Intern | Digital Transformation & IT Department</span>
        </div>
        <div style="margin-bottom: 10px; display: flex; justify-content: space-between; align-items: center; font-size: 16px">
            <span>Manager: <a href="fisher.jia@bayer.com" target="_blank" style="color: #35705D; text-decoration: underline;">Fisher Jia</a></span>
        </div>
        <div style="font-size: 14px;">
          <em>My role</em>:<br>
        </div>
          <div style="font-size: 14px; margin-left: 15px;">
            <li>Analyze e-commerce market share, applying basic methods to study various Chinese e-commerce brands. Collect data through a crawler, perform data analysis, and discuss findings with the Department of Marketing.</li>
            <li>Investigate the root causes of failures in an OCR technology designed for small ticket image recognition. Serve as the project manager to improve and test the system's design.</li>
            <li>Support the company's training department by: i) Designing a survey system, including creating survey questionnaires, web pages, QR codes, and conducting final testing; ii) Using the Python pandas package to clean survey data collected by colleagues; iii) Providing technical support for live broadcasts, such as testing the live video environment in the initial stages and monitoring the live broadcast. Additionally, prepare a final technical report.</li>
        </div>
    </div>
<div><hr style="border: 0; border-top: 1px solid #dcdcdc; margin: 10px 0;"></div>


  <div style="font-family: Arial, sans-serif; line-height: 1.6; margin: 12px;">
        <div style="margin-bottom: 10px; display: flex; justify-content: space-between; align-items: center; font-size: 16px;">
            <span>
                2021.06 - 2021.08, 
              <a href="https://www.iquanzhan.com/about.html" target="_blank" style="color: #35705D; text-decoration: underline;">Fullstack Intelligence Co., Ltd</a>, SH, CN
            </span>     
            <span>Algorithm Engineer | Smart City Infrastructure Solution </span>
        </div>
        <div style="margin-bottom: 10px; display: flex; justify-content: space-between; align-items: center; font-size: 16px">
            <span>Manager: <a href="fahedxy@gmail.com" target="_blank" style="color: #35705D; text-decoration: underline;">Hao Chen</a></span><br>
        </div>
        <div style="font-size: 14px;">
          <em>Goal</em>: The system enables real-time video collection and analysis of vehicles on the road, providing accurate and timely insights into traffic conditions.<br>
          <em>My role</em>:<br>
        </div>
        <div style="font-size: 14px; margin-left: 15px;">
          <li>Real-time video monitoring from buses and taxis facilitates traffic road inspections through the integration of accessed video data.</li>
          <li>AI-powered vision systems detect road issues, generate problem reports, and automatically notify responsible units for resolution.</li>
          <li>The PDCA closed-loop inspection framework enhances highway administration and ensures road safety and efficiency.</li>
        </div>
    </div>
<div><hr style="border: 0; border-top: 1px solid #dcdcdc; margin: 10px 0;"></div>




<br>
<span class='anchor' id='services-activities'></span>
# <span style="font-weight: bold; color: #654f4fcb; font-size: 28px;">🛎️ Services and Activities</span>

# <span style="font-size: 20px;">Community and Journal Reviewers</span>
<ul style="font-family: Arial, sans-serif;">
  <li>The 33rd International Conference on Computer Communications and Networks (ICCCN 2024)</li>
  <li>IEEE Transactions on Intelligent Transportation Systems (T-ITS)</li>
</ul>

# <span style="font-size: 20px;">University Service</span>
<ul style="font-family: Arial, sans-serif;">
  <li>Graduate Chaperone to guide a team of 14 undergraduate female students to the Grace Hopper Celebration of Women in Computing (<a href="https://ghc.anitab.org/" target="_blank" style=" color: #35705D; text-decoration: none;">GHC</a>), Philadelphia, PA, USA, 2024.</li>
</ul>

# <span style="font-size: 20px;">Activities</span>
<ul style="font-family: Arial, sans-serif;">
  <li>TribeCTF – W&M’s first Capture-the-Flag (<a href="https://tribectf.cs.wm.edu/" target="_blank" style="color: #35705D; text-decoration: none;">CTF</a>), Williamsburg, VA, USA.</li>
  <li>Capital Women in Computing (<a href="https://capwic.org/" target="_blank" style="color: #35705D; text-decoration: none;">CAPWIC</a>) conference, VA, USA, 2024.</li>
</ul>
<div><hr style="border: 0; border-top: 1px solid #dcdcdc; margin: 10px 0;"></div>

<br>
<span class='anchor' id='honors-awards'></span>
<span style="font-weight: bold; color: #654f4fcb; font-size: 28px;">🎖 Honors and Awards</span>
<ul style="font-family: Arial, sans-serif;">
  <li>Dec 2024: NSF ACM/IEEE Symposium on Edge Computing (SEC) Student Travel Grant.</li>
  <li>Oct 2024: International Student Opportunity Scholarship at William & Mary.</li>
  <li>July 2024: Research Assistant Fellowship, Vehicle Computing Lab.</li>
  <li>May 2024: NSF IEEE International Conference on Mobility: Operations, Services, and Technologies (MOST) Student Travel Grant Award.</li>
  <div><hr style="border: 0; border-top: 1px solid #dcdcdc; margin: 10px 0;"></div>
  
  <li>2019 - 2023: Academic Excellence Scholarship, Shanghai Dianji Univ., Top 1%.</li>
  <li>July 2023: Big Model Innovation and Creative Applications Competition, Top 1%.</li>
  <li>May 2022 - May 2023: Research Leader in Shanghai 2022 College Student Innovation Competition.</li>
  <li>2021: “MathorCup” National Mathematical Modeling Challenge for undergraduate.</li>
  <li>May 2020 - May 2021: Research member in Shanghai 2020 College Student Innovation Competition.</li>
</ul>
<div><hr style="border: 0; border-top: 1px solid #dcdcdc; margin: 10px 0;"></div>


<span class='anchor' id='educations'></span>
# <span style="font-weight: bold; color: #654f4fcb; font-size: 28px;">📖 Educations</span>

<ul style="font-family: Arial, sans-serif;">
  <li>2023.09 - current, William & Mary, USA.</li>
  <li>2019.09 - 2023.06, Shanghai Dianji University, China.</li>
</ul>
<div><hr style="border: 0; border-top: 1px solid #dcdcdc; margin: 10px 0;"></div>
