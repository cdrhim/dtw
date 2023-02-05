# Translink Deep Tech Weekly (DTW)

🌍 Website: [link](https://cdrhim.github.io/dtw/)\
💾 Repository: [link](https://www.github.com/cdrhim/dtw/)

- [DTW-1](##week_1_(DTW-1))



## Week 1 (DTW-1)

ChatGPT를 분해해 보면 그 구조가 어떻게 되어있냐?
강화학습+Azure AI Infrastructure 활용
(예전에 2021년 GPT-3를 베타 테스트 웨이팅리스트 기회가 와서 했을 때에 비해 ChatGPT는 더 긍정적인 톤의 답을 내놓는다는 생각이 들었다.)

특이점: 과거 General Adversarial Networks (GAN)이나 

우려점: 데이터를 Stack Overflow와 같은 타 사이트를 scrapping 해서 integrity 이슈가 생길 수 있다. 보통 웹사이트 상 프론트 부분인 UI에서 보여지는 어떤 데이터든 scrapping 하는 것에는 법적인 문제가 없지만, 이를 통해 제3자가 2차 수익을 내는 것은 문제가 있을 수 있다.

또, 틀린답을 내놓을 수 있기 때문에 output에 대해 검증을 하는 수단이 또 필요하게 될 것이다. 

서버 비용이 학습하고 추론하는 데에 많이 쓰여 research preview 때만 제공하려던 무료서비스를 지속할 수 없고, 결국 올해 2023년 마이크로소프트가 인수하면서 유료로 전환이 되었다.
마이크로소프트가 Open AI 인수함에 따라 AWS, GCP, Azure의 market share도 달라질 수 있을 것이라 생각한다. 또, Bing에게 적용이 될 ChatGPT를 통해 사용량이 늘 것이라 Google의 market share도 줄 수 있을 것이다.

ChatGPT는 결국 GPT-3 기반으로 같은 수의 파라미터로 만들어진 GPT-3.5와 동의어로 생각할 수 있고, InstructGPT의 연장선이라 볼 수 있다. 곧 파라미터 수가 확 늘은 GPT-4가 만들어질 것이라 계속해서 발전된 형태의 output을 기대할 수 있다. 2021년 이후의 더 최신 데이터를 input으로 넣는지에 따라 더 좋은 결과를 낼 수 있다.

Multi-modal learning AI를 통해 앞으로 text의 한 도메인 학습보다 text-to-image (DALL-E), text-to-video 등의 generative AI가 더 흥행할 것이다.

2023년 서울대 이교구 교수님의 Supertone (Mnet, SBS 등에서 죽은 가수가 환생해 최신곡을 커버함)을 인수한 하이브처럼 최신 리서치에 관심이 있는 스타트업이 경쟁력이 있고 IP확보에 유리할 것이다. Supertone과 같은 경우에는 글쓴이 본인의 옆 연구실이고, 수업을 들은 바로 음성 뿐만이 아니라 안무라든지의 연구가 수년 간 이루어졌다.

voice.ai를 보면 유튜브에 쇼츠로 일반인이 일론 머스크의 비디오로 다른 목소리(모간 프리먼, 조 바이든, 앤드류 테이트 등 50여 가지)와 sync를 맞출 수 있는 예시들을 유저들이 꾸준히 체험해 볼 수 있게끔 한다. 다른 비디오에서는 Roblox에 voice.ai를 통해 목소리를 입히는 법을 알려준다. 각종 창의적인 수단으로 B2C, B2B 홍보하는 스타트업들이 ChatGPT와 같은 폭팔적 인기를 끌 수 있을 것이다.
https://youtube.com/shorts/S84CgeVCNO8?feature=share

Midjourney

NVIDIA와 같은 경우에도 눈의 시선을 자연스럽게 보정해주는 기술(Broadcase)이 개발이 되었고, 2023년 현재 1.4버전 서비스 중이다.
https://www.nvidia.com/en-us/geforce/news/jan-2023-nvidia-broadcast-update/

Microsoft Teams가 Notion보다 인기가 많아진 이유는 이미 선점하고 있던 Windows의 distribution 때문.


최신 핫한 논문들

논문을 내는 곳 중에 컨퍼런스와 저널 등이 있고, IF가 높을수록 더 명성이 높은 곳이라 할 수 있다.
ICLR, NIPS, ICML, AAAI 등이 있다.
https://scholar.google.es/citations?view_op=top_venues&hl=en&vq=eng_artificialintelligence

논문을 제출해서 accept되고 출판될 때 바로 핫해지는 논문이 있는가 하면, 한참 후에 유명해지는 논문들도 있다. 보통은 산업에서 쓰이기 전에 이미 논문 기술들이 유명해진다.

<!---
Week 2
About all the licenses that could be included in open source software (Apache 2.0, etc.).

-->
