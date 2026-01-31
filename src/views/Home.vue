<!-- src/views/Home.vue -->
<template>
  <div>
    <NavBar :logo-text="logoText" :links="navLinks" />

    <main class="main-container">
      <ProfileHeader
        name="Martin Zhou"
        title="Undergraduate Student"
        photo-src="/assets/figs/zty.jpg"
      />

      <!-- Summary / Biography -->
      <Section id="summary" title="Summary">
        <div class="card">
          <p style="text-align: justify">
            I am an undergraduate student in
            <strong>Intelligent Software and Engineering</strong> at
            <a href="https://www.nju.edu.cn/" target="_blank"
              >Nanjing University</a
            >, with a strong interest in
            <strong>Artificial Intelligence</strong> and
            <strong>Big Data Analysis</strong>. My experience spans AI system
            software development, model optimization, image processing, and
            industrial Machine Learning applications. I am a keen learner and
            practitioner, motivated by curiosity and innovation, and aim to
            build a solid academic foundation to pursue <strong>AGI</strong> in
            the long term.
          </p>
        </div>
      </Section>

      <!-- Education -->
      <Section id="education" title="Education">
        <div class="card">
          <ul class="edu-list">
            <li>
              <div class="edu-header">
                <div>
                  <strong>Nanjing University</strong>,
                  <span>Nanjing / Suzhou, China</span>
                </div>
                <div class="edu-time">Sept. 2022 – Present</div>
              </div>
              <div class="edu-body">
                <div>
                  <em>B.Eng. in Intelligent Software and Engineering</em>
                </div>
                <div>GPA: <strong>4.3 / 5.0</strong></div>
                <div>
                  Key Coursework: Data Structures, Machine Learning, Operating
                  Systems, Natural Language Processing, Pattern Recognition
                  &amp; Computer Vision, Advanced Algorithms, Internet
                  Computing.
                </div>
              </div>
            </li>

            <li>
              <div class="edu-header">
                <div>
                  <strong
                    >Northwest Polytechnical University Affiliated High
                    School</strong
                  >,
                  <span>Xi'an, China</span>
                </div>
                <div class="edu-time">Sept. 2019 – Jul. 2022</div>
              </div>
              <div class="edu-body">
                <div>Rank: <strong>Top 5%</strong></div>
                <div>
                  Competitions: Chinese High School Mathematics League (2nd
                  Prize), 2021 &amp; 2022.
                </div>
              </div>
            </li>
          </ul>
        </div>
      </Section>

      <!-- News (简要，用 card 列表风格) -->
      <Section id="news" title="News">
        <div class="card">
          <ul class="news-list">
            <li>
              <span class="news-date">2025:</span>
              Preparing graduate applications and strengthening research
              experience in
              <strong>Machine Learning</strong>, <strong>LLMs</strong>, and
              <strong>AI systems</strong>.
            </li>
            <li>
              <span class="news-date">2024–2025:</span>
              Participated in COMAP Mathematical Contest in Modeling (MCM/ICM)
              as
              <strong>Successful Participant (S Prize)</strong>.
            </li>
            <li>
              <span class="news-date">2024:</span>
              Awarded the <strong>People's Scholarship</strong> at Nanjing
              University for excellent academic performance.
            </li>
          </ul>
        </div>
      </Section>

      <!-- Research Interests -->
      <Section id="research" title="Research Interests">
        <div class="card">
          <ul class="interest-list">
            <li>
              <strong
                >Brain-inspired Artificial Intelligence &amp; Human-level
                Cognition:</strong
              >
              interest in few-shot learning, continual learning, and cognitive
              models that move towards more human-like intelligence.
            </li>
            <li>
              <strong>Efficient Large-scale AI Systems:</strong>
              model compression, LLM training and optimization, distributed
              training, and hardware–software co-design for deploying models in
              real-world applications.
            </li>
            <li>
              <strong>Applied AI in Industrial and Medical Scenarios:</strong>
              industrial Machine Learning (e.g., predictive maintenance) and
              AI-assisted medical imaging (e.g., ultrasound diagnostics).
            </li>
          </ul>
        </div>
      </Section>

      <!-- Internship Experience -->
      <Section id="internship" title="Internship Experience">
        <div class="card">
          <ul class="project-list">
            <li class="project-item">
              <div class="project-header">
                <div>
                  <strong>GE Aerospace</strong> – Data Science Analyst Intern
                </div>
                <div class="project-tag">Industrial ML in Production</div>
              </div>
              <p class="project-desc">
                Engaged with <strong>Industrial IoT</strong> scenarios,
                developing, testing, and analyzing data science models such as
                predictive maintenance and failure analysis. Supported
                data-driven decisions for optimizing asset efficiency and
                reliability in industrial environments.
              </p>
            </li>

            <li class="project-item">
              <div class="project-header">
                <div>
                  <strong>Bailead Tech</strong> – Software Engineer Intern
                </div>
                <div class="project-tag">AI Software Development</div>
              </div>
              <p class="project-desc">
                Collaborated with physicians from multiple hospitals and
                mechanical engineers to analyze medical ultrasound images and
                build an AI-assisted diagnostic system. Responsible for
                AI-related software development and testing using
                <strong>C/C++</strong> and <strong>Python</strong>, focusing on
                imaging pipeline and model integration.
              </p>
            </li>
          </ul>
        </div>
      </Section>

      <!-- Research and Academic Projects -->
      <Section id="projects-research" title="Research and Academic Projects">
        <div class="card">
          <ol class="pub-list">
            <!-- DDCPS project -->
            <li class="pub-item">
              <a href="https://github.com/ZhizhengFu/DDCPS" target="_blank">
                DDCPS: Drift Diffusion Model for Chess Player Skill Evaluation
              </a>
              <span class="spacer"></span>
              <span class="authors"> <strong>Project Lead</strong> </span><br />
              <span class="venue">
                Target submission: IEEE Conference on Games (CIG). </span
              ><br />
              <div class="buttons">
                <a
                  class="button button4"
                  href="https://github.com/ZhizhengFu/DDCPS"
                  target="_blank"
                >
                  Code
                </a>
              </div>
              <p class="project-desc">
                Led a study applying
                <strong>Drift–Diffusion Models (DDM)</strong> to chess skill
                assessment. Demonstrated that by tracking move quality
                (Centipawn Loss, CPL) across 20–30 games, the method can provide
                faster and more stable estimates than traditional Elo rating in
                early stages.
              </p>
            </li>

            <!-- LibFewShot contribution -->
            <li class="pub-item">
              <a href="https://github.com/RL-VIG/LibFewShot" target="_blank">
                LibFewShot – Open-source Contribution
              </a>
              <span class="spacer"></span>
              <span class="authors">
                Contributor to the <strong>LibFewShot</strong> library (TPAMI
                2023). </span
              ><br />
              <span class="venue">
                Focused on reproduction and architectural refactoring of the
                MeTAL method (ICCV 2021). </span
              ><br />
              <div class="buttons">
                <a
                  class="button button4"
                  href="https://github.com/RL-VIG/LibFewShot"
                  target="_blank"
                >
                  Code
                </a>
              </div>
              <p class="project-desc">
                Worked on improving the reliability and code structure of the
                <strong>LibFewShot</strong> library, including reproduction and
                refactoring of the MeTAL few-shot learning method, to make the
                framework more accessible and robust for the research community.
              </p>
            </li>

            <!-- Ultrasound project -->
            <li class="pub-item">
              <span class="pub-title">
                Autonomous AI Ultrasound Diagnostic System
              </span>
              <span class="spacer"></span>
              <span class="authors">
                Project Lead, Provincial Innovation Project; two invention
                patent applications. </span
              ><br />
              <span class="venue">
                AI-based ultrasound scanning guidance and diagnostic record
                generation. </span
              ><br />
              <p class="project-desc">
                Led the development of an AI-assisted ultrasound diagnostic
                system, responsible for image processing and statistical
                analysis. Proposed methods for
                <strong>automatic scanning guidance</strong> and
                <strong>automatic diagnostic record generation</strong>, which
                resulted in two invention patent applications on ultrasound
                scanning and diagnostic workflows.
              </p>
            </li>
          </ol>
        </div>
      </Section>

      <!-- LLM & Software Engineering Projects -->
      <Section id="projects-llm" title="LLM and Software Engineering Projects">
        <div class="card">
          <ol class="pub-list">
            <!-- LLM pipeline -->
            <li class="pub-item">
              <a href="https://github.com/Aquila-zhou1/LLM" target="_blank">
                End-to-End LLM Training and Optimization Pipeline
              </a>
              <span class="spacer"></span>
              <span class="authors">
                Independent project on large language model training and
                optimization. </span
              ><br />
              <span class="venue">
                Pre-training, SFT, LoRA, RLHF; training optimization with
                DeepSpeed ZeRO-2 and DPO. </span
              ><br />
              <div class="buttons">
                <a
                  class="button button4"
                  href="https://github.com/Aquila-zhou1/LLM"
                  target="_blank"
                >
                  Code
                </a>
              </div>
              <p class="project-desc">
                Implemented the full LLM lifecycle, including pre-training,
                supervised fine-tuning, parameter-efficient fine-tuning (LoRA),
                and RLHF-style optimization. Achieved
                <strong>&gt;50% memory reduction</strong> in 4-GPU training
                using <strong>DeepSpeed ZeRO-2</strong> and
                <strong>FP16 + CPU offload</strong>, and explored
                <strong>DPO (Direct Preference Optimization)</strong> to improve
                stability and efficiency over PPO-based RLHF. Used
                <strong>Weights &amp; Biases</strong> for experiment tracking
                and visualization.
              </p>
            </li>

            <!-- RAG platform -->
            <li class="pub-item">
              <a href="https://github.com/horserr/rag-chat" target="_blank">
                Nanjing University Handbook RAG Platform
              </a>
              <span class="spacer"></span>
              <span class="authors">
                Full-stack development with FastAPI, SpringBoot, and DevOps
                practices. </span
              ><br />
              <span class="venue">
                Retrieval-Augmented Generation system for campus information
                Q&amp;A. </span
              ><br />
              <div class="buttons">
                <a
                  class="button button4"
                  href="https://github.com/horserr/rag-chat"
                  target="_blank"
                >
                  Code
                </a>
              </div>
              <p class="project-desc">
                Designed and implemented a RAG-based Q&amp;A system for the
                Nanjing University handbook, combining
                <strong>FastAPI</strong> services, a
                <strong>SpringBoot</strong> backend, and a CI/CD pipeline with
                <strong>Docker</strong> on campus cloud resources. Realized
                continuous integration and automated deployment to support
                iterative development and reliable service delivery.
              </p>
            </li>

            <!-- HarmonyOS app -->
            <li class="pub-item">
              <a
                href="https://github.com/KevinXu11155/Know-Ur-Weather"
                target="_blank"
              >
                Know-Ur-Weather – HarmonyOS Application
              </a>
              <span class="spacer"></span>
              <span class="authors">
                Collaboration on API integration and system-level optimization. </span
              ><br />
              <span class="venue">
                Weather application with offline caching and multi-threaded data
                processing. </span
              ><br />
              <div class="buttons">
                <a
                  class="button button4"
                  href="https://github.com/KevinXu11155/Know-Ur-Weather"
                  target="_blank"
                >
                  Code
                </a>
              </div>
              <p class="project-desc">
                Developed API integration, <strong>offline caching</strong>, and
                data synchronization using HarmonyOS
                <strong>Preferences</strong>. Implemented multi-threading
                optimization with <code>@ohos.taskpool</code> to improve
                responsiveness, and integrated the Gaode Map API to provide
                location-aware weather information.
              </p>
            </li>
          </ol>
        </div>
      </Section>

      <!-- Skills -->
      <Section id="skills" title="Technical Skills">
        <div class="card">
          <ul class="skill-list">
            <li>
              <strong>Programming:</strong>
              C/C++, Python, Java, Julia, MATLAB; solid foundation in algorithms
              and data structures.
            </li>
            <li>
              <strong>AI/ML Frameworks:</strong>
              PyTorch, HuggingFace Transformers, DeepSpeed, Weights &amp;
              Biases, Scikit-learn; familiar with LLM training and optimization
              techniques.
            </li>
            <li>
              <strong>Backend &amp; Tools:</strong>
              SpringBoot, FastAPI, Docker, Linux, Git, CI/CD; basic
              understanding of distributed systems concepts.
            </li>
          </ul>
        </div>
      </Section>

      <!-- Patents -->
      <Section id="patents" title="Patents">
        <div class="card">
          <ul class="patent-list">
            <li>
              Method and system capable of automatically scanning and diagnosis
              with Ultrasonic (CN202310690905.5)
            </li>
            <li>
              Electronic equipment and storage medium for automatic Ultrasonic
              probe and inspection (CN202310690903.6)
            </li>
          </ul>
        </div>
      </Section>

      <!-- Honors -->
      <Section id="honors" title="Honors and Awards">
        <div class="card">
          <ul class="honor-list">
            <li>
              <strong>Competitions:</strong>
              Successful Participant (S Prize), COMAP Mathematical Contest in
              Modeling (MCM/ICM), 2024 &amp; 2025.
            </li>
            <li>
              <strong>Scholarship:</strong>
              People's Scholarship (2024), awarded to top academic performers at
              Nanjing University.
            </li>
            <li>
              <strong>Activities:</strong>
              Organized multiple campus club concerts and cultural events.
            </li>
          </ul>
        </div>
      </Section>

      <!-- Extra-curricular -->
      <Section id="extra" title="Extra-curricular Activities">
        <div class="card">
          <ul class="extra-list">
            <li><strong>Piano:</strong> Level 10 certified.</li>
            <li><strong>Chess:</strong> Amateur level 4.</li>
            <li>
              <strong>Other interests:</strong> Swimming, biking, and reading.
            </li>
          </ul>
        </div>
      </Section>

      <AppFooter />
    </main>
  </div>
</template>

<script setup lang="ts">
import NavBar from "@/components/NavBar.vue";
import ProfileHeader from "@/components/ProfileHeader.vue";
import Section from "@/components/Section.vue";
import AppFooter from "@/components/AppFooter.vue";

const logoText = "Martin Tianyuan Zhou";

const navLinks = [
  { id: "summary", label: "Summary" },
  { id: "education", label: "Education" },
  { id: "research", label: "Research" },
  { id: "projects-research", label: "Research Projects" },
  { id: "projects-llm", label: "LLM & SE" },
  { id: "skills", label: "Skills" },
  { id: "honors", label: "Honors" },
  { id: "extra", label: "Activities" },
];
</script>

<style scoped>
.main-container {
  max-width: 960px;
  margin: 25px auto 40px;
  padding: 0 20px 40px 20px;
  background-color: #ffffff;              /* 整个内容区域白色 */
  box-shadow: 0 2px 10px rgba(0,0,0,0.08);/* 白纸浮在灰底上 */
  border-radius: 6px;
}

/* 通用 card 容器，延续 Wenbin Li 紧凑但有悬浮感的风格 */
.card {
  background-color: #ffffff;
  border-radius: 6px;
  padding: 14px 16px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.06);
  margin-bottom: 1em;
  transition: box-shadow 0.2s ease, transform 0.2s ease;
}

.card:hover {
  box-shadow: 0 4px 14px rgba(0,0,0,0.12);
  transform: translateY(-1px);
}

/* Education */
.edu-list {
  list-style: none;
  padding-left: 0;
  margin: 0;
}

.edu-list li + li {
  margin-top: 0.8em;
  padding-top: 0.6em;
  border-top: 1px dotted #e0e0e0;
}

.edu-header {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  gap: 8px;
}

.edu-header span {
  font-size: 0.9em;
  color: #666;
}

.edu-time {
  font-size: 0.9em;
  color: #777;
}

.edu-body {
  margin-top: 0.2em;
  font-size: 0.95em;
  line-height: 1.3;
}

/* News */
.news-list {
  margin: 0;
  padding-left: 20px;
}

.news-list li {
  margin-bottom: 0.4em;
  line-height: 1.3;
}

.news-date {
  font-weight: 500;
}

/* Research Interests */
.interest-list {
  margin: 0;
  padding-left: 20px;
}

.interest-list li {
  margin-bottom: 0.4em;
  line-height: 1.3;
}

/* Projects as card-like items */
.project-list {
  list-style: none;
  padding-left: 0;
  margin: 0;
}

.project-item + project-item {
  margin-top: 0.8em;
}

.project-item {
  padding: 8px 4px;
  border-bottom: 1px dotted #e0e0e0;
}

.project-header {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  gap: 8px;
  margin-bottom: 2px;
}

.project-tag {
  font-size: 0.8em;
  padding: 2px 6px;
  border-radius: 4px;
  background-color: #d6eaf8;
  color: #022b6d;
}

.project-desc {
  margin-top: 4px;
  font-size: 0.95em;
  line-height: 1.3;
}

/* Publication-style lists (reuse Wenbin Li 风格) */
.pub-list {
  margin-top: 0.3em;
  padding-left: 20px;
}

.pub-item {
  padding: 8px;
  margin-bottom: 8px;
  border-radius: 5px;
  border-bottom: 1px dotted #eaeaea;
  transition: all 0.2s ease;
}

.pub-item a:first-of-type {
  font-weight: 500;
  color: #2a4a8c;
  text-decoration: none;
  transition: color 0.3s;
}

.pub-item a:first-of-type:hover {
  color: #3498db;
  text-decoration: underline;
}

.pub-title {
  font-weight: 500;
  color: #2a4a8c;
}

.spacer {
  display: block;
  height: 5px;
}

.venue {
  color: #e74c3c;
}

.buttons {
  margin-top: 2px;
}

/* Buttons */
.button {
  font-family: Georgia, serif;
  background-color: #d6eaf8;
  border: none;
  color: #022b6d;
  padding: 4px 8px;
  text-decoration: none;
  display: inline-block;
  font-size: 0.85em;
  margin: 2px 3px;
  border-radius: 4px;
  transition: all 0.3s ease;
}

.button:hover {
  background-color: #aed6f1;
  transform: translateY(-2px);
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

/* Hover 效果：左边条 + 阴影，延续 Wenbin Li 风格 */
.pub-item:hover {
  background-color: #f5f5f5;
  border-left: 5px solid #4285f4;
  box-shadow: 0 5px 15px rgba(66, 133, 244, 0.2);
  transform: translateX(5px);
  padding-left: 10px;
}

/* Skills / patents / honors / extras */
.skill-list,
.patent-list,
.honor-list,
.extra-list {
  margin: 0;
  padding-left: 20px;
}

.skill-list li,
.patent-list li,
.honor-list li,
.extra-list li {
  margin-bottom: 0.35em;
  line-height: 1.3;
}

@media (max-width: 768px) {
  .edu-header,
  .project-header {
    flex-direction: column;
    align-items: flex-start;
  }
}
</style>
