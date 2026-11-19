![Terrence Chuwe · AI & Automation Engineer · Harare, Zimbabwe](assets/portfolio.svg)

I build AI tools for the people who use them day to day. At Cassava Technologies, I work on network reporting, retrieval-augmented generation, and GPU inference. Before that, I built backend services and UiPath automations for teams across Southern and East Africa.

[LinkedIn](https://www.linkedin.com/in/terrence-chuwe-1a5615190/) · [Email](mailto:tchuwe41@gmail.com)

## Selected projects

| Project | What you can explore |
| --- | --- |
| [StoreBridge](https://github.com/PAPA-CHUWE/storebridge) | Follow a supplier listing into an AI-assisted product draft, then through Saleor to the Next.js storefront. The README maps the implemented flow and the roadmap. |
| [VektorCode](https://github.com/PAPA-CHUWE/vektorcode) | A Python coding agent that connects to an OpenAI-compatible endpoint to inspect a project, edit files, and run tests. |
| [Climate Risk & Health Prediction](https://github.com/PAPA-CHUWE/Climate-Risk-and-Health-Prediction-Challenge) | A Zindi project exploring how climate and health data can help predict climate-sensitive mortality in Uganda. |

## Skills

![Retrieval-augmented generation](assets/skill-0.svg) ![LLM integration](assets/skill-1.svg) ![AI agents](assets/skill-2.svg) ![GPU inference](assets/skill-3.svg) ![Workflow automation](assets/skill-4.svg) ![Backend APIs](assets/skill-5.svg) ![Model evaluation](assets/skill-6.svg) ![CI/CD](assets/skill-7.svg)

## Tech stack

**Languages & APIs**  
![python,go,dotnet,fastapi](https://skillicons.dev/icons?i=python,go,dotnet,fastapi)

**Web & data**  
![react,nextjs,postgres](https://skillicons.dev/icons?i=react,nextjs,postgres)

**Build & delivery**  
![docker,git,githubactions](https://skillicons.dev/icons?i=docker,git,githubactions)

## RAG architecture

A reference design for answering questions from a document collection. Indexing happens when documents change. At query time, retrieval supplies passages and source IDs for the model’s answer.

```mermaid
flowchart TD
    D["Source documents"] --> C["Split into passages"]
    C --> E["Embed passages"]
    E --> I[("Vector index + source IDs")]
    Q["User question"] --> V["Embed question"]
    V --> R["Retrieve relevant passages"]
    I --> R
    R --> P["Assemble prompt"]
    Q --> P
    P --> L["Language model"]
    L --> A["Answer with sources"]
```
