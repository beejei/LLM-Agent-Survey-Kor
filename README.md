# LLM 기반 자율 에이전트에 대한 조사

![Growth Trend](assets/trend.png)

자율 에이전트는 자체 지침을 통해 특정 목표를 달성하도록 설계되었습니다. 대규모 언어 모델(LLM)의 출현과 성장으로 이러한 자율 에이전트의 기본 컨트롤러로 LLM을 활용하는 경향이 증가하고 있습니다. 이 분야의 이전 연구들은 주목할만한 성공을 달성했지만, 체계적인 분석에는 별도의 노력이 거의 기울여지지 않았습니다. 이 격차를 메우기 위해 우리는 LLM 기반 자율 에이전트의 구축, 응용 및 평가에 초점을 맞춘 종합적인 조사 연구를 수행합니다. 특히, 우리는 AI 에이전트의 핵심 구성 요소인 프로필 모듈, 메모리 모듈, 계획 모듈 및 행동 모듈을 탐구합니다. 그런 다음 자연 과학, 사회 과학 및 공학 분야에서 LLM 기반 자율 에이전트의 응용을 조사합니다. 이어서 이 분야에서 사용된 평가 전략에 대한 논의를 심화하며, 주관적 및 객관적 방법을 모두 포함합니다. 우리의 조사는 연구자와 실무자에게 통찰력, 관련 참고 문헌 및 이 흥미롭고 빠르게 진화하는 분야에 대한 지속적인 업데이트를 제공하는 자원으로서의 역할을 하기를 목표로 합니다.

**📍 이는 LLM 기반 자율 에이전트 분야에서 처음으로 발표된 조사 논문입니다.**

논문 링크:  [LLM 기반 자율 에이전트에 대한 조사](https://journal.hep.com.cn/fcs/EN/10.1007/s11704-024-40231-1) 


## Update Records
- 🔥  [2024년 3월 25일] 우리의 조사 논문이 컴퓨터 과학 전선에 의해 받아들여졌으며, 이는 LLM 기반 에이전트 분야에서 처음으로 발표된 조사 논문입니다.
  
- 🔥 [2023년 9월 28일] 우리는 Neurips 2023에 받아들여진 LLM 기반 에이전트 관련 논문을 정리하고 요약하여 LLM-Agent-Paper-Digest 저장소에 컴파일했습니다. 이 저장소는 앞으로 받아들여진 에이전트 관련 논문으로 계속 업데이트될 것입니다.
  
- 🔥 [2023년 9월 8일] 우리의 조사의 두 번째 버전이 arXiv에 출시되었습니다.
   <details>
    <summary>업데이트된 내용</summary>

    -  **📚 추가 참고 문헌**
        - We have added 31 new works until 9/1/2023 to make the survey more comprehensive and up-to-date.

    -  **📊 새로운 그림**
        - **그림 3:** 다양한 계획 접근법 사이의 차이점과 유사점을 설명하는 새로운 그림입니다. 이를 통해 다른 계획 방법 사이의 비교를 더 명확하게 이해할 수 있습니다.
        ![single-path and multi-path reasoning](assets/planning.png)
        - **그림 4:** "기계 학습 시대"에서 "대규모 언어 모델 시대" 그리고 "에이전트 시대"로의 모델 능력 획득의 진화 경로를 설명하는 새로운 그림입니다. 특히, "메커니즘 엔지니어링"이라는 새로운 개념이 도입되었으며, 이는 "파라미터 학습" 및 "프롬프트 엔지니어링"과 함께 이 진화 경로의 일부를 형성합니다.
        ![Capabilities Acquisition](assets/capability.png)

    -  **🔍 최적화된 분류 시스템**
        - 우리는 조사의 분류 체계를 약간 수정하여 더 논리적이고 조직적으로 만들었습니다.
  </details>

- 🔥 [2023년 8월 23일] 우리의 조사의 첫 번째 버전이 arXiv에 출시되었습니다.<br>
          

<!--omit in the toc-->
## Table of Content

<!-- - [Growth Trend in the Field of LLM-based Autonomous Agent](#-growth-trend-of-llm-based-autonomous-agent)-->
- [🤖 Construction of LLM-based Autonomous Agent](#-construction-of-llm-based-autonomous-agent)
- [📍 Applications of LLM-based Autonomous Agent](#-applications-of-llm-based-autonomous-agent)
- [📊 Evaluation on LLM-based Autonomous Agent](#-evaluation-on-llm-based-autonomous-agent)
- [🌐 More Comprehensive Summarization](#-more-comprehensive-summarization)
- [👨‍👨‍👧‍👦 Maintainers](#-maintainers)
- [📚 Citation](#-citation)
- [💪 How to Contribute](#-how-to-contribute)
- [🫡 Acknowledgement](#-acknowledgement)
- [📧 Contact Us](#-contact-us)


<!-- ## 📚 Growth Trend in the Field of LLM-based Autonomous Agent
![Growth Trend](assets/trend.png)
<hr>  -->

<!-- ## 📋 Structure of the Survey
![Structure](assets/survey.png)
<hr> -->

## 🤖 Construction of LLM-based Autonomous Agent
![Architecture Design](assets/architecture-1.png)

<table>
    <tr>
        <td rowspan='2'align='center'>Model</td>
        <td rowspan='2'align='center'>Profile</td>
        <td colspan='2'align='center'>Memory</td>
        <td rowspan='2'align='center'>Planning</td>
        <td rowspan='2'align='center'>Action</td>
        <td rowspan='2'align='center'>CA</td>  
        <td rowspan='2'align='center'>Paper</td>
        <td rowspan='2'align='center'>Code</td>
    </tr>
    <tr>
        <td align='center'>Operation</td>
        <td align='center'>Structure</td>
    </tr>
    <tr>
        <td align='center'>WebGPT</td>
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>w/ fine-tuning</td> 
        <td align='center'><a href="https://arxiv.org/abs/2112.09332">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>SayCan</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/o feedback</td> 
        <td align='center'>w/o tools</td> 
        <td align='center'>w/o fine-tuning</td>  
        <td align='center'><a href="https://arxiv.org/abs/2204.01691">Paper</a></td>
        <td align='center'><a href="https://say-can.github.io/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>MRKL</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/o feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2205.00445">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Inner Monologue</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/o tools</td> 
        <td align='center'>w/o fine-tuning</td> 
        <td align='center'><a href="https://arxiv.org/abs/2207.05608">Paper</a></td>
        <td align='center'><a href="https://innermonologue.github.io/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Social Simulacra</td>  
        <td align='center'>GPT-Generated</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/o tools</td> 
        <td align='center'>-</td>   
        <td align='center'><a href="https://arxiv.org/abs/2208.04024">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ReAct</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>w/ fine-tuning</td> 
        <td align='center'><a href="https://arxiv.org/abs/2210.03629">Paper</a></td>
        <td align='center'><a href="https://github.com/ysymyth/ReAct">Code</a></td>
    </tr>
        <tr>
        <td align='center'>LLM Planner</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/o tools</td> 
        <td align='center'>Environment feedback</td> 
        <td align='center'><a href="https://arxiv.org/abs/2212.04088">Paper</a></td>
        <td align='center'><a href="https://dki-lab.github.io/LLM-Planner">Code</a></td>
    </tr>
    <tr>
        <td align='center'>MALLM</td> 
        <td align='center'>-</td>  
        <td align='center'>Read/Write</td> 
        <td align='center'>Hybrid</td> 
        <td align='center'>-</td>  
        <td align='center'>w/o tools</td> 
        <td align='center'>-</td>   
        <td align='center'><a href="https://arxiv.org/abs/2301.04589">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>aiflows</td> 
        <td align='center'>-</td>  
        <td align='center'>Read/Write/<br>Reflection</td> 
        <td align='center'>Hybrid</td> 
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>-</td>   
        <td align='center'><a href="https://arxiv.org/abs/2308.01285">Paper</a></td>
        <td align='center'><a href="https://github.com/epfl-dlab/aiflows">Code</a></td>
    </tr>
    <tr>
        <td align='center'>DEPS</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/o tools</td> 
        <td align='center'>w/o fine-tuning</td> 
        <td align='center'><a href="https://arxiv.org/abs/2302.01560">Paper</a></td>
        <td align='center'><a href="https://github.com/CraftJarvis/MC-Planner">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Toolformer</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/o feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>w/ fine-tuning</td>  
        <td align='center'><a href="https://arxiv.org/abs/2302.04761">Paper</a></td>
        <td align='center'><a href="https://github.com/lucidrains/toolformer-pytorch">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Reflexion</td> 
        <td align='center'>-</td>  
        <td align='center'>Read/Write/<br>Reflection</td> 
        <td align='center'>Hybrid</td> 
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/o tools</td> 
        <td align='center'>w/o fine-tuning</td> 
        <td align='center'><a href="https://arxiv.org/abs/2303.11366">Paper</a></td>
        <td align='center'><a href="https://github.com/noahshinn024/reflexion">Code</a></td>
    </tr>
    <tr>
        <td align='center'>CAMEL</td> 
        <td align='center'>Handcrafting & GPT-Generated</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td>  
        <td align='center'>w/o tools</td> 
        <td align='center'>-</td>  
        <td align='center'><a href="https://arxiv.org/abs/2303.17760">Paper</a></td>
        <td align='center'><a href="https://github.com/camel-ai/camel">Code</a></td>
    </tr>
    <tr>
        <td align='center'>API-Bank</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td>  
        <td align='center'>w/ tools</td> 
        <td align='center'>w/o fine-tuning</td> 
        <td align='center'><a href="https://arxiv.org/abs/2304.08244">Paper</a></td>
        <td align='center'><a href="url">-</a></td>
    </tr>
       </tr>
        <tr>
        <td align='center'>Chameleon</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/o feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>-</td> 
        <td align='center'><a href="https://arxiv.org/abs/2304.09842">Paper</a></td>
        <td align='center'><a href="https://chameleon-llm.github.io/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>ViperGPT</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ tools</td>  
        <td align='center'>-</td>  
        <td align='center'><a href="https://arxiv.org/abs/2303.08128">Paper</a></td>
        <td align='center'><a href="https://github.com/cvlab-columbia/viper">Code</a></td>
    </tr>
    <tr>
        <td align='center'>HuggingGPT</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td> 
        <td align='center'>Unified</td> 
        <td align='center'>w/o feedback</td>  
        <td align='center'>w/ tools</td> 
        <td align='center'>-</td>  
        <td align='center'><a href="https://arxiv.org/abs/2303.17580">Paper</a></td>
        <td align='center'><a href="https://huggingface.co/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Generative Agents</td> 
        <td align='center'>Handcrafting</td> 
        <td align='center'>Read/Write/<br>Reflection</td> 
        <td align='center'>Hybrid</td> 
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/o tools</td>  
        <td align='center'>-</td>   
        <td align='center'><a href="https://arxiv.org/abs/2304.03442">Paper</a></td>
        <td align='center'><a href="https://github.com/joonspk-research/generative_agents">Code</a></td>
    </tr>
    <tr>
        <td align='center'>LLM+P</td> 
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/o feedback</td> 
        <td align='center'>w/o tools</td> 
        <td align='center'>-</td>   
        <td align='center'><a href="https://arxiv.org/abs/2304.11477">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ChemCrow</td>
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>w/ feedback</td>
        <td align='center'>w/ tools</td>
        <td align='center'>-</td> 
        <td align='center'><a href="https://arxiv.org/abs/2304.05376">Paper</a></td>
        <td align='center'><a href="https://github.com/ur-whitelab/chemcrow-public">Code</a></td>
    </tr>
    <tr>
        <td align='center'>OpenAGI</td>
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>w/ feedback</td>
        <td align='center'>w/ tools</td>
        <td align='center'>w/ fine-tuning</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.04370">Paper</a></td>
        <td align='center'><a href="https://github.com/agiresearch/OpenAGI/blob/main/README.md">Code</a></td>
    </tr>
    <tr>
        <td align='center'>AutoGPT</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write</td>
        <td align='center'>Hybrid</td>
        <td align='center'>w/ feedback</td>
        <td align='center'>w/ tools</td>
        <td align='center'>w/o fine-tuning</td> 
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/Significant-Gravitas/Auto-GPT">Code</a></td>
    </tr>
    <tr>
        <td align='center'>SCM</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write</td>
        <td align='center'>Hybrid</td>
        <td align='center'>-</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>-</td> 
        <td align='center'><a href="https://arxiv.org/abs/2304.13343">Paper</a></td>
        <td align='center'><a href="https://github.com/wbbeyourself/scm4llms">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Socially Alignment</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write</td>
        <td align='center'>Hybrid</td>
        <td align='center'>-</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>Example</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.16960">Paper</a></td>
        <td align='center'><a href="https://github.com/agi-templar/Stable-Alignment">Code</a></td>
    </tr>
    <tr>
        <td align='center'>GITM</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write/<br>Reflection</td>
        <td align='center'>Hybrid</td>
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>w/ fine-tuning</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.17144">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenGVLab/GITM">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Voyager</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write/<br>Reflection</td>
        <td align='center'>Hybrid</td>
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>w/o fine-tuning</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.16291">Paper</a></td>
        <td align='center'><a href="https://github.com/MineDojo/Voyager">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Introspective Tips</td>
        <td align='center'>-</td> 
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>w/ feedback</td>
        <td align='center'>w/o tools</td>
        <td align='center'>w/o fine-tuning</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.11598">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>RET-LLM</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write</td>
        <td align='center'>Hybrid</td>
        <td align='center'>-</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>w/ fine-tuning</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.14322">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ChatDB</td>
        <td align='center'>-</td> 
        <td align='center'>Read/Write</td> 
        <td align='center'>Hybrid</td> 
        <td align='center'>w/ feedback</td>
        <td align='center'>w/ tools</td> 
        <td align='center'>-</td> 
        <td align='center'><a href="https://arxiv.org/abs/2306.03901">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>S3</td> 
        <td align='center'>Dataset alignment</td>
        <td align='center'>Read/Write/<br>Reflection</td>
        <td align='center'>Hybrid</td> 
        <td align='center'>-</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>w/ fine-tuning</td> 
        <td align='center'><a href="https://arxiv.org/abs/2307.14984">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ChatDev</td>
        <td align='center'>Handcrafting</td>
        <td align='center'>Read/Write/<br>Reflection</td>
        <td align='center'>Hybrid</td>
        <td align='center'>w/ feedback</td>
        <td align='center'>w/o tools</td>
        <td align='center'>w/o fine-tuning</td> 
        <td align='center'><a href="https://arxiv.org/abs/2307.07924">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenBMB/ChatDev">Code</a></td>
    </tr>
    <tr>
        <td align='center'>ToolLLM</td>
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>-</td> 
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/ tools</td>
        <td align='center'>w/ fine-tuning</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.16789">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenBMB/ToolBench">Code</a></td>
    </tr>
    <tr>
        <td align='center'>MemoryBank</td> 
        <td align='center'>-</td> 
        <td align='center'>Read/Write/<br>Reflection</td>
        <td align='center'>Hybrid</td>
        <td align='center'>-</td> 
        <td align='center'>w/o tools</td>
        <td align='center'>-</td> 
        <td align='center'><a href="https://arxiv.org/abs/2305.10250">Paper</a></td>
        <td align='center'><a href="https://github.com/zhongwanjun/MemoryBank-SiliconFriend">Code</a></td>
    </tr>
    <tr>
        <td align='center'>MetaGPT</td>
        <td align='center'>Handcrafting</td>
        <td align='center'>Read/Write/<br>Reflection</td>
        <td align='center'>Hybrid</td>
        <td align='center'>w/ feedback</td>
        <td align='center'>w/ tools</td>
        <td align='center'>-</td>  
        <td align='center'><a href="https://arxiv.org/abs/2308.00352">Paper</a></td>
        <td align='center'><a href="https://github.com/geekan/MetaGPT">Code</a></td>
    </tr>
   <tr>
        <td align='center'>LEO</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>-</td>  
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/o tools</td> 
        <td align='center'>w/ fine-tuning</td> 
        <td align='center'><a href="https://arxiv.org/abs/2311.12871">Paper</a></td>
        <td align='center'><a href="https://embodied-generalist.github.io">Code</a></td>
    </tr>
   <tr>
        <td align='center'>JARVIS-1</td>  
        <td align='center'>-</td>  
        <td align='center'>Read/Write/<br>Reflection</td>
        <td align='center'>Hybrid</td>
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>w/o fine-tuning</td> 
        <td align='center'><a href="https://arxiv.org/abs/2311.05997">Paper</a></td>
        <td align='center'><a href="https://github.com/CraftJarvis/JARVIS-1">Code</a></td>
    </tr>
   <tr>
        <td align='center'>CLOVA</td>  
        <td align='center'>-</td>  
        <td align='center'>Read/Write/<br>Reflection</td>
        <td align='center'>Hybrid</td>
        <td align='center'>w/ feedback</td> 
        <td align='center'>w/ tools</td> 
        <td align='center'>w/ fine-tuning</td> 
        <td align='center'><a href="https://arxiv.org/abs/2312.10908">Paper</a></td>
        <td align='center'><a href="https://clova-tool.github.io/">Code</a></td>
    </tr>
</table>

* More papers can be found at [More comprehensive Summarization](#-more-comprehensive-summarization).
* CA means the strategy of model capability acquisition.

## 📍 Applications of LLM-based Autonomous Agent

<table>
    <tr>
        <td align='center'>Title</td>
        <td align='center'>Social Science </td>
        <td align='center'>Natural Science </td>
        <td align='center'>Engineering</td>
        <td align='center'>Paper</td>
        <td align='center'>Code</td>
    </tr>
    <tr>
        <td align='center'>Drori et al.</td>
        <td align='center'>-</td>
        <td align='center'>Science Education</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2112.15594">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>SayCan</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/pdf/2204.01691">Paper</a></td>
        <td align='center'><a href="https://say-can.github.io/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Inner monologue</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/pdf/2207.05608">Paper</a></td>
        <td align='center'><a href="https://innermonologue.github.io/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Language-Planners</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2201.07207">Paper</a></td>
        <td align='center'><a href="https://github.com/huangwl18/language-planner">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Social Simulacra</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2208.04024">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>TE</td>
        <td align='center'>Psychology </td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2208.10264">Paper</a></td>
        <td align='center'><a href="https://github.com/gatiaher/using-large-language-models-to-replicate-human-subject-studies">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Out of One</td>
        <td align='center'>Political Science and Economy</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/pdf/2209.06899">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>LIBRO</td>
        <td align='center'>CS&SE</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/pdf/2209.11515">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Blind Judgement</td>
        <td align='center'>Jurisprudence</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/pdf/2301.05327.pdf">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Horton</td>
        <td align='center'>Political Science and Economy</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2301.07543">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>DECKARD</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2301.12050">Paper</a></td>
        <td align='center'><a href="https://github.com/DeckardAgent/deckard">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Planner-Actor-Reporter</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2302.00763">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>DEPS</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2302.01560">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>RCI</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2303.17491">Paper</a></td>
        <td align='center'><a href="https://github.com/posgnu/rci-agent">Code</a></td>
    </tr>  
    <tr>
        <td align='center'>Generative Agents</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.03442">Paper</a></td>
        <td align='center'><a href="https://github.com/joonspk-research/generative_agents">Code</a></td>
    </tr>    
    <tr>
        <td align='center'>SCG</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/pdf/2304.07590">Paper</a></td>
        <td align='center'>-</td>
    </tr>   
    <tr>
        <td align='center'>IGLU</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Civil Engineering</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.10750">Paper</a></td>
        <td align='center'>-</td>
    </tr>   
    <tr>
        <td align='center'>IELLM</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Industrial Automation</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.14354">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>ChemCrow</td>
        <td align='center'>-</td>
        <td align='center'>Document and Data Management;<br>Documentation, Data Managent;<br>Science Education<br></td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.05332">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>Boiko et al.</td>
        <td align='center'>-</td>
        <td align='center'>Document and Data Management;<br>Documentation, Data Managent;<br>Science Education<br></td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.14354">Paper</a></td>
        <td align='center'>-</td>
    </tr>   
    <tr>
        <td align='center'>GPT4IA</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Industrial Automation</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.14721">Paper</a></td>
        <td align='center'><a href="https://github.com/YuchenXia/GPT4IndustrialAutomation">Code</a></td>
    </tr>  
    <tr>
        <td align='center'>Self-collaboration</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.07590">Paper</a></td>
        <td align='center'>-</td>
    </tr>   
    <tr>
        <td align='center'>E2WM</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.10626">Paper</a></td>
        <td align='center'><a href=" szxiangjn/world-model-for-language-model (github.com)">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Akata et al.</td>
        <td align='center'>Psychology </td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.16867">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Ziems et al.</td>
        <td align='center'>Psychology;<br>Political Science and Economy;<br>Research Assistant </td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.03514">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>AgentVerse</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.10848">Paper</a></td>
        <td align='center'><a href="https://githuba.com/OpenBMB/AgentVerse">Code</a></td>
    </tr>     
    <tr>
        <td align='center'>SmolModels</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/smol-ai/developer">Code</a></td>
    </tr> 
    <tr>
        <td align='center'>TidyBot</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.05658">Paper</a></td>
        <td align='center'><a href="https://github.com/jimmyyhwu/tidybot">Code</a></td>
    </tr>  
    <tr>
        <td align='center'>PET</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.02412">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>Voyager</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.16291">Paper</a></td>
        <td align='center'><a href="https://github.com/MineDojo/Voyager">Code</a></td>
    </tr>  
    <tr>
        <td align='center'>GITM</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.17144">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenGVLab/GITM">Code</a></td>
    </tr>  
    <tr>
        <td align='center'>NLSOM</td>
        <td align='center'>-</td>
        <td align='center'>Science Education</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.17066">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>LLM4RL</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2306.03604">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>GPT Engineer</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/AntonOsika/gpt-engineer">Code</a></td>
    </tr> 
    <tr>
        <td align='center'>Grossman et al.</td>
        <td align='center'>-</td>
        <td align='center'>Experiment Assistant;<br>Science Education</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://www.science.org/doi/full/10.1126/science.adi1778">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>SQL-PALM</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2306.00739">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>REMEMBER</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2306.07929">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>DemoGPT</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://github.com/melih-unsal/DemoGPT">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Chatlaw</td>
        <td align='center'>Jurisprudence</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2306.16092">Paper</a></td>
        <td align='center'><a href="https://github.com/PKU-YuanGroup/ChatLaw">Code</a></td>
    </tr>  
    <tr>
        <td align='center'>RestGPT</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2306.06624">Paper</a></td>
        <td align='center'><a href="https://restgpt.github.io">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Dialogue shaping</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.15833">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>TaPA</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.01848">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>Ma et al.</td>
        <td align='center'>Psychology </td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.15810">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Math Agents</td>
        <td align='center'>-</td>
        <td align='center'>Science Education</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/pdf/2307.02502">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>SocialAI School</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.07871">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>Unified Agent</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.09668">Paper</a></td>
        <td align='center'>-</td>
    </tr>   
    <tr>
        <td align='center'>Wiliams et al.</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.04986">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>Li et al.</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.10337">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>S3</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.14984">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>Dialogue Shaping</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/pdf/2307.15833.pdf">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>RoCo</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.06135">Paper</a></td>
        <td align='center'><a href="https://project-roco.github.io/">Code</a></td>
    </tr> 
    <tr>
        <td align='center'>Sayplan</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.04738">Paper</a></td>
        <td align='center'><a href="https://sayplan.github.io/">Code</a></td>
    </tr> 
    <tr>
        <td align='center'>aiflows</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS & SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.01285">Paper</a></td>
        <td align='center'><a href="https://github.com/epfl-dlab/aiflows">Code</a></td>
    </tr>
    <tr>
        <td align='center'>ToolLLM</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.16789">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenBMB/ToolBench">Code</a></td>
    </tr> 
    <tr>
        <td align='center'>ChatDEV</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.07924">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>Chao et al.</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.13304v1">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>AgentSims</td>
        <td align='center'>Social Simulation</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.04026">Paper</a></td>
        <td align='center'><a href="https://github.com/py499372727/AgentSims">Code</a></td>
    </tr>
    <tr>
        <td align='center'>ChatMOF</td>
        <td align='center'>-</td>
        <td align='center'>Document and Data Management;<br>Science Education</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/pdf/2308.01423">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>MetaGPT</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.00352">Paper</a></td>
        <td align='center'><a href="https://github.com/geekan/MetaGPT">Code</a></td>
    </tr> 
    <tr>
        <td align='center'>Codehelp</td>
        <td align='center'>-</td>
        <td align='center'>Science Education</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.06921">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>AutoGen</td>
        <td align='center'>-</td>
        <td align='center'>Science Education</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.08155">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>RAH</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.09904">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>DB-GPT</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.05481">Paper</a></td>
        <td align='center'><a href="https://github.com/TsinghuaDatabaseGroup/DB-GPT">Code</a></td>
    </tr>  
    <tr>
        <td align='center'>RecMind</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.14296">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>ChatEDA</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.10204">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
    <tr>
        <td align='center'>InteRecAgent</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.16505">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>PentestGPT</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.06782">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>Codehelp</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.06921">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ProAgent</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
     	<td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.11339">Paper</a></td>
        <td align='center'>-</td>
    </tr> 
    <tr>
        <td align='center'>MindAgent</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2309.09971">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
   <tr>
        <td align='center'>LEO</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2311.12871">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
   <tr>
        <td align='center'>JARVIS-1</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>Robotics & Embodied AI</td>
        <td align='center'><a href="https://arxiv.org/abs/2311.05997">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
   <tr>
        <td align='center'>CLOVA</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'>CS&SE</td>
        <td align='center'><a href="https://arxiv.org/abs/2312.10908">Paper</a></td>
        <td align='center'>-</td>
    </tr>  
</table>

* More papers can be found at [More comprehensive Summarization](#-more-comprehensive-summarization).

## 📊 Evaluation on LLM-based Autonomous Agent

<table>
    <tr>
        <td align='center'>Model</td>
        <td align='center'>Subjective </td>
        <td align='center'>Objective </td>
        <td align='center'>Benchmark</td>
        <td align='center'>Paper</td>
        <td align='center'>Code</td>
    </tr>
    <tr>
        <td align='center'>WebShop</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation;<br> Multi-task Evaluation </td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2207.01206">Paper</a></td>
        <td align='center'><a href="https://github.com/princeton-nlp/webshop">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Social Simulacra</td>
        <td align='center'>Human Annotation</td>
        <td align='center'>Social Evaluation</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2208.04024">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>TE</td>
        <td align='center'>-</td>
        <td align='center'>Social Evaluation</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2208.10264">Paper</a></td>
        <td align='center'><a href="https://github.com/GatiAher/UsingLarge-Language-Models-to-Replicate-Human-Subject-Studies">Code</a></td>
    </tr>
    <tr>
        <td align='center'>LIBRO</td>
        <td align='center'>-</td>
        <td align='center'>Software Testing</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2209.11515">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>ReAct</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2210.03629">Paper</a></td>
        <td align='center'><a href="https://github.com/ysymyth/ReAct">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Out of One, Many</td>
        <td align='center'>Turing Test</td>
        <td align='center'>Social Evaluation;<br> Multi-task Evaluation</td>
        <td align='center'>-</td>        
        <td align='center'><a href="https://arxiv.org/abs/2209.06899">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>DEPS</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2302.01560">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Jalil et al.</td>
        <td align='center'>-</td>
        <td align='center'>Software Testing</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2302.03287">Paper</a></td>
        <td align='center'><a href="https://github.com/sajedjalil/ChatGPT-Software-Testing-Stud">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Reflexion</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation;<br> Multi-task Evaluation</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2303.11366">Paper</a></td>
        <td align='center'><a href="https://github.com/noahshinn024/reflexion">Code</a></td>
    </tr>
    <tr>
        <td align='center'>IGLU</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.10750">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Generative Agents</td>
        <td align='center'> Human Annoation;<br>Turing Test</td>
        <td align='center'>-</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2304.03442">Paper</a></td>
        <td align='center'><a href="https://github.com/joonspk-research/generative_agents">Code</a></td>
    </tr>
    <tr>
        <td align='center'>ToolBench</td>
        <td align='center'>Human Annoation</td>
        <td align='center'>Multi-task Evalution</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.16789">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenBMB/ToolBench">Code</a></td>
    </tr>
    <tr>
        <td align='center'>GITM</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.17144">Paper</a></td>
        <td align='center'><a href="https://github.com/OpenGVLab/GITM">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Two-Failures</td>
        <td align='center'>-</td>
        <td align='center'>Multi-task Evalution</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.14279">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Voyager</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.16291">Paper</a></td>
        <td align='center'><a href="https://github.com/MineDojo/Voyager">Code</a></td>
    </tr>
    <tr>
        <td align='center'>SocKET</td>
        <td align='center'>-</td>
        <td align='center'>Social Evaluation;<br>Multi-task Evaluation </td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.14938">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>Mobile-Env</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation;<br> Multi-task Evaluation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.08144">Paper</a></td>
        <td align='center'><a href="https://github.com/X-LANCE/Mobile-Env">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Clembench</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation;<br> Multi-task Evaluation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.13455">Paper</a></td>
        <td align='center'><a href="https://github.com/clp-research/clembench">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Mind2Web</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation;<br> Multi-task Evaluation</td>
        <td align='center'>&check;</td>
        <td align='center'>06/2023</td>
        <td align='center'><a href="https://arxiv.org/abs/2306.06070">Paper</a></td>
        <td align='center'><a href="https://github.com/OSU-NLP-Group/Mind2Web">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Dialop</td>
        <td align='center'>-</td>
        <td align='center'>Social Evaluation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2305.20076">Paper</a></td>
        <td align='center'><a href="https://github.com/jlin816/dialop">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Feldt et al.</td>
        <td align='center'>-</td>
        <td align='center'>Software Testing</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2306.05152">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>CO-LLM</td>
        <td align='center'>Human Annoation</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.02485">Paper</a></td>
        <td align='center'><a href="https://vis-www.cs.umass.edu/Co-LLM-Agents/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Tachikuma</td>
        <td align='center'>Human Annoation</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.12573">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>WebArena</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.13854">Paper</a></td>
        <td align='center'><a href="https://github.com/web-arena-x/webarena">Code</a></td>
    </tr>
    <tr>
        <td align='center'>RocoBench</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation;<br> Social Evaluation;<br> Multi-task Evaluation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2307.04738">Paper</a></td>
        <td align='center'><a href="https://project-roco.github.io/">Code</a></td>
    </tr>
    <tr>
        <td align='center'>AgentSims</td>
        <td align='center'>-</td>
        <td align='center'>Social Evaluation</td>
        <td align='center'>-</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.04026">Paper</a></td>
        <td align='center'><a href="https://github.com/py499372727/AgentSims">Code</a></td>
    </tr>
    <tr>
        <td align='center'>AgentBench</td>
        <td align='center'>-</td>
        <td align='center'>Multi-task Evaluation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.03688">Paper</a></td>
        <td align='center'><a href="https://github.com/thudm/agentbench">Code</a></td>
    </tr>
    <tr>
        <td align='center'>BOLAA</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation;<br>Multi-task Evaluation;<br>Software Testing</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.05960">Paper</a></td>
        <td align='center'><a href="https://github.com/salesforce/BOLAA">Code</a></td>
    </tr>
    <tr>
        <td align='center'>Gentopia</td>
        <td align='center'>-</td>
        <td align='center'>Isolated Reasoning;<br> Multi-task Evaluation </td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.04030">Paper</a></td>
        <td align='center'><a href="https://github.com/Gentopia-AI/Gentopia">Code</a></td>
    </tr>
    <tr>
        <td align='center'>EmotionBench</td>
        <td align='center'>Human Annotation</td>
        <td align='center'>-</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.03656">Paper</a></td>
        <td align='center'><a href="https://github.com/CUHK-ARISE/EmotionBench">Code</a></td>
    </tr>
    <tr>
        <td align='center'>PTB</td>
        <td align='center'>-</td>
        <td align='center'>Software Testing </td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2308.06782">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>MintBench</td>
        <td align='center'>-</td>
        <td align='center'>Multi-task Evaluation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2309.10691">Paper</a></td>
        <td align='center'><a href="https://github.com/xingyaoww/mint-bench">Code</a></td>
    </tr>
    <tr>
        <td align='center'>MindAgent</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation;<br>Multi-task Evaluation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2309.09971">Paper</a></td>
        <td align='center'>-</td>
    </tr>
    <tr>
        <td align='center'>JARVIS-1</td>
        <td align='center'>-</td>
        <td align='center'>Environment Simulation</td>
        <td align='center'>&check;</td>
        <td align='center'><a href="https://arxiv.org/abs/2311.05997">Paper</a></td>
        <td align='center'>-</td>
    </tr>
</table>

* More papers can be found at [More comprehensive Summarization](#-more-comprehensive-summarization).

<hr>

## 🌐 더 포괄적인 요약

우리는 LLM 기반 에이전트와 관련된 더 포괄적인 논문들을 포함하고 있는 [인터랙티브 테이블](https://abyssinian-molybdenum-f76.notion.site/237e9f7515d543c0922c74f4c3012a77?v=0a309e53d6454afcbe7a5a7e169be0f9&pvs=4)을 유지하고 있습니다. 이 테이블에는 태그, 저자, 출판 날짜 등의 세부 정보가 포함되어 있어 관심 있는 논문을 정렬, 필터링 및 찾을 수 있습니다.

![Complete Table](assets/table.png)

## 👨‍👨‍👧‍👦 유지 관리자
- Lei Wang@[Paitesanshi](https://github.com/Paitesanshi)
- Chen Ma@[Uily](https://github.com/Yilu114)
- Xueyang Feng@[XueyangFeng](https://github.com/XueyangFeng)

## 📚 인용
이 조사가 유용하다고 생각되면 우리의 논문을 인용해 주세요:
```
@misc{wang2023survey,
      title={A Survey on Large Language Model based Autonomous Agents}, 
      author={Lei Wang and Chen Ma and Xueyang Feng and Zeyu Zhang and Hao Yang and Jingsen Zhang and Zhiyuan Chen and Jiakai Tang and Xu Chen and Yankai Lin and Wayne Xin Zhao and Zhewei Wei and Ji-Rong Wen},
      year={2023},
      eprint={2308.11432},
      archivePrefix={arXiv},
      primaryClass={cs.AI}
}
```


## 💪 기여하는 방법
포함되어야 할 논문이 있거나 관련 연구를 알고 있다면, pull requests, 이슈, 이메일 또는 기타 적절한 방법을 통해 기여해 주세요.


## 🫡 감사의 말
이 조사에 귀중한 제안과 기여를 한 다음 사람들에게 감사합니다:
- Yifan Song[@Yifan-Song793](https://github.com/Yifan-Song793)
- Qichen Zhao[@Andrewzh112](https://github.com/Andrewzh112)
- Ikko E. Ashimine[@eltociear](https://github.com/eltociear)


## 📧 연락처
질문이나 제안이 있으면 다음을 통해 연락해 주세요:
- 이메일: wanglei154@ruc.edu.cn, xu.chen@ruc.edu.cn


