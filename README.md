# Translink Deep Tech Weekly (DTW)

๐ Website: [link](https://cdrhim.github.io/dtw/)\
๐พ Repository: [link](https://www.github.com/cdrhim/dtw/)



- [DTW-1](#week-1-dtw-1)

----------

## Week 1 (DTW-1)

- ChatGPT๋ฅผ ๋ถํดํด ๋ณด๋ฉด ๊ทธ **๊ตฌ์กฐ**๊ฐ ์ด๋ป๊ฒ ๋์ด์์๊น?
<br>
<br>

![chatgpt-diagram](./assets/img/chatgpt_diagram.svg)
*OpenAI. (2022, Nov. 30). ChatGPT: Optimizing Language Models for Dialogue. https://openai.com/blog/chatgpt/*

1. ์ธํฐ๋ท ์ 570GB ์ ๋์ ํ์คํธ ๋ฐ์ดํฐ<sub>(๋๋ 3000์ต ๊ฐ์ ๋จ์ด๋ค)</sub>๋ฅผ ์ถ์ถํจ
2. ์ด ๋ฐ์ดํฐ๋ฅผ ํ์ฉํ์ฌ prompt (question) ๋ฐ์ดํฐ์์ ๊ตฌ์ถํจ
3. ๋ ์ด๋ธ๋งํ๋ ์ฌ๋์ด prompt (question) ๋ฐ์ดํฐ์์ผ๋ก๋ถํฐ output (answer)์ ๋ง๋ค์ด ๋ชจ์์ง ๋ฐ์ดํฐ๋ก ์ง๋ํ์ต๋ชจ๋ธ์ ํ๋ จํจ<sub>(์ง๋ํ์ต์ input๊ณผ output ์์ ๋ฐ์ดํฐ์์ด ์์ ์์ ํ์ต ๊ฐ๋ฅํ ๋จธ์ ๋ฌ๋ ๊ธฐ๋ฒ์ด๋ค)</sub>
4. ํ์ output์ ๋ํ ์ฌ๋์ ์ง์ ์ ์ธ ํผ๋๋ฐฑ<sub>(best-to-worst๋ฅผ ์์ฐจ์ ์ผ๋ก ๋์ด)</sub>์ ํตํ ๋ณด์๋ชจ๋ธ์ ํ๋ จํจ<sub>(๋ณด์๋ชจ๋ธ์ ๊ฐํํ์ต์ ํ๊ธฐ ์ํด ํ์ฉ๋๋ค)</sub>
5. ์ด๋์ ๋ ์ํ๋ ์์ค์ ๋ต์ ๋ด๊ธฐ๊น์ง ๊ณ์๋ ๊ฐํํ์ต์ ์งํ

*(On Prem์ด ์๋ Azure AI Infrastructure๋ฅผ ํตํด ๋ชจ๋  ํ์ต์ด ์ด๋ฃจ์ด์ง์๋ค.)* \
*(๊ฐํํ์ต์ ๊ณผ๊ฑฐ ์ํ๊ณ ๋ฅผ ๊ฐ๋ฐํ  ๋์๋ ์ฐ์ธ ๊ธฐ์ ์ด๋ค. ๋ณดํต ๊ฒ์์น๋ถ์ ๊ฐ์ ํ์คํฌ์์ ๊ฐํํ์ต์ด ์ฐ์ธ๋ค.)* \
*(์์ ์ 2021๋ GPT-3๋ฅผ ๋ฒ ํ ํ์คํธ ์จ์ดํ๋ฆฌ์คํธ ๊ธฐํ๊ฐ ์์ ํ์ ๋์ ๋นํด ChatGPT๋ ๋ ๊ธ์ ์ ์ธ ํค์ ๋ต์ ๋ด๋๋๋ค๋ ์๊ฐ์ด ๋ค์ด์ ์ต๊ทผ 2022๋ 3์๋ถํฐ ์ ์ฉํ ๊ฐํํ์ต([link](https://arxiv.org/abs/2203.02155))์ ๋ ๊ธ์ ์ ์ด๊ฒ ๋ง๋  ํจ๊ณผ๊ฐ ์์ ์ ์๊ฒ ๋ค ์๊ฐํ๋ค.)*

๋ฐ๋ผ์, ์ง๋ํ์ต๊ณผ ๊ฐํํ์ต์ ์ ์ ํ ์กฐํฉํ ๋ฐฉ์์ผ๋ก ChatGPT๋ฅผ ํ์ตํ๋ค๊ณ  ๋ณผ ์ ์๋ค.

- ChatGPT๋ ๊ฒฐ๊ตญ GPT-3 ๊ธฐ๋ฐ์ผ๋ก ๊ฐ์ ์์ 175B ํ๋ผ๋ฏธํฐ๋ก ๋ง๋ค์ด์ง GPT-3.5์ ๋์์ด๋ก ์๊ฐํ  ์ ์๊ณ , InstructGPT์ ์ฐ์ฅ์ ์ด๋ผ ๋ณผ ์ ์๋ค. 2018๋์ ๋ํ๋ GPT-1 ("Improving Language Understanding by Generative Pre-training", [link](https://s3-us-west-2.amazonaws.com/openai-assets/research-covers/language-unsupervised/language_understanding_paper.pdf))๋ถํฐ ์์ํด, 2019๋ GPT-2 ("Language Models are unsupervised multitask learners", [link](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf)), 2020๋ GPT-3 ("Language Models are few shot learners", [link](https://arxiv.org/pdf/2005.14165.pdf)), ๊ทธ๋ฆฌ๊ณ  GPT-3.5๊น์ง ๋ฐ์ ํ๋ค. ๊ณง ํ๋ผ๋ฏธํฐ ์๊ฐ ํ ๋์ GPT-4๊ฐ ๋ง๋ค์ด์ง ๊ฒ์ด๋ผ ๊ณ์ํด์ ๋ฐ์ ๋ ํํ์ output์ ๊ธฐ๋ํ  ์ ์๋ค. **GPT-4๋ 2023๋ 1๋ถ๊ธฐ์ ๋์ฌ ์ ์๋ค**๋ ์ถ์ธก์ด ์๋ค([link](https://the-decoder.com/gpt-4-only-launches-when-it-is-safe-and-responsible/)). ๊ทธ๋ฆฌ๊ณ  2021๋ ์ดํ์ ๋ ์ต์  ๋ฐ์ดํฐ๋ฅผ input์ผ๋ก ๋ฃ๋์ง์ ๋ฐ๋ผ ๋ ์ข์ ๊ฒฐ๊ณผ๋ฅผ ๋ผ ์ ์๋ค.

![gpt3-gpt4](./assets/img/gpt3-gpt4.jpg)
*Acquisition.com LLC. https://acquisition.com*

- **ChatGPT ํน์ด์ **: ๊ณผ๊ฑฐ ์ ๋ชํด์ง๊ณ  ํ์ฌ๊น์ง ์ฐ์ด๋ ์ธ๊ณต์ง๋ฅ ๊ธฐ์ ๋ค์ธ ์ด์ ๊ตฟํ ๋ก์ฐ(Ian Goodfellow)์ 2014๋ [General Adversarial Networks (GAN)](https://arxiv.org/abs/1406.2661)์ด๋ ๋ฒค ๋ฐ๋ ํ(Ben Mildenhall), ๋งคํ ํ์(Matthew Tancik)์ 2020๋ [NeRF (Neural Radiance Fields)](https://arxiv.org/abs/2003.08934)๋ ์ ๋ช ํํ๋ ์ ๋์ ํตํด ๋ฐํ๋ ๊ธฐ์ ๋ค์ด๋ค. GAN์ NIPS๋ ํํ์ accept์ด ๋์๊ณ , NeRF๋ ECCV์ Oral ๋ถ๋ฌธ์์ Best Paper ์์ ๋ฐ์๋ค. ์ด๋ฅผ ํตํด ์ด๋ค ์ฌ๋์ด ์ฒ์ ์ด๋ค ๊ธฐ์ ์ ์ ์ํ๋์ง ์ ์ ์๊ณ , ์ด๋ค ๋งค์ฒด์ ๊ฒ์ฆ์ ๊ฑฐ์ณค๋์ง ์ ์ ์์๋ค. ๊ทธ๋ฌ๋ ChatGPT๋ ์ด์ ๋ค๋ฅด๊ฒ ์ ๋ช ํํ๋ ์ ๋์ peer review๋ก ์ 3์์ ๊ฒ์ฆ์ ๊ฑฐ์น์ง ์์๋ค๋ ํน์ด์ ์ด ์๊ณ , ํ๊ณ๊ฐ ์๋ ๊ธฐ์์์ ๋ฐํ๋ ์ ์ด ํฅ๋ฏธ๋ก์ธ ์ ์๋ค. ๊ทธ๋ฆฌ๊ณ  source code๊ฐ ์คํ์์ค๋ก ๊ณต๊ฐ๋์ง ์์ ์ ํํ ์ด๋ค ๊ธฐ์กด ๋ฐ์ดํฐ๋ ๋ชจ๋ธ์ ํ์ฉํ๊ณ  ํ๋์ง ์ ์ ์๋ค. ์ธ๋๋ ์ด์ผ๊ธฐ์ง๋ง ํฅ๋ฏธ๋กญ๊ฒ๋ ์ด์ ๊ตฟํ ๋ก์ฐ๋ 2016๋ 3์์ OpenAI์ ์กฐ์ธ์ ํ๋ค๊ฐ 11๊ฐ์ ๋ง์ ๋ค์ Google Research๋ก ๋ณต๊ทํ ๋ฐ๊ฐ ์๋ค. SOTA <sub>(์ต๊ณ ์ฑ๋ฅ, State of the Art)</sub>๋ฅผ ๋ด๋ ์ธ๊ธฐ ๊ธฐ์ ๋ก๋ ์ด๋ค ํ์คํฌ([link](https://paperswithcode.com/sota))์ ์ ์ฉํ๋๋์ ๋ฐ๋ผ ๋ค์ํ ์ข๋ฅ๋ค์ด ์์ผ๋ฉฐ, Transformers, CLIP, GAN, NeRF, Stable Diffusion ๋ฑ์ด ๋ํ์ ์ผ๋ก ์๋ค.

- **ChatGPT ์ฐ๋ ค์ **: ๋ฐ์ดํฐ๋ฅผ Stack Overflow์ ๊ฐ์ ํ ์ฌ์ดํธ๋ฅผ scrapping ๋๋ crawling ํด์ integrity ์ด์๊ฐ ์๊ธธ ์ ์๋ค. ๋ณดํต ์น์ฌ์ดํธ ์ ํ๋ก ํธ ๋ถ๋ถ์ธ UI์์ ๋ณด์ฌ์ง๋ ์ด๋ค ๋ฐ์ดํฐ๋  scrapping ํ๋ ๊ฒ์๋ ๋ฒ์ ์ธ ๋ฌธ์ ๊ฐ ์์ง๋ง, ์ด๋ฅผ ํตํด ์ 3์๊ฐ 2์ฐจ ์์ต์ ๋ด๋ ๊ฒ์ ๋ฌธ์ ๊ฐ ์์ ์ ์๋ค. **Y Combinator์์๋ ์ด์ (2023๋ 2์ 5์ผ) ์ด์ ๋ํ ๋๊ธํ ๋ก ๋ ์์๋๋ฐ, ์ค์ ChatGPT์ ํฉ๋ฒ์ฑ์ ๋ํด ์ด๋ค ๋ต์ด ๋ด๋ ค์ง ์ํ๊ฐ ์๋๋ค**([link](https://news.ycombinator.com/item?id=34664998&ref=upstract.com)). ๋, ํ๋ฆฐ๋ต์ ๋ด๋์ ์ ์๊ธฐ ๋๋ฌธ์ output์ ๋ํด ๊ฒ์ฆ์ ํ๋ ์๋จ์ด ๋ ํ์ํ๊ฒ ๋  ๊ฒ์ด๋ค.

- ์๋ฒ ๋น์ฉ์ด ํ์ตํ๊ณ  ์ถ๋ก ํ๋ ๋ฐ์ ๋ง์ด ์ฐ์ฌ research preview ๋๋ง ์ ๊ณตํ๋ ค๋ ๋ฌด๋ฃ์๋น์ค๋ฅผ ์ง์ํ  ์ ์์ ์ ์๊ณ , ๊ฒฐ๊ตญ ์ฌํด 2023๋ ๋ง์ดํฌ๋ก์ํํธ๊ฐ 29B USD valuation์ผ๋ก 10B USD ํฌ์๋ก 49% ์ง๋ถ์ ๋์ฃผ์ฃผ๊ฐ ๋๋ฉด์ ์ ๋ฃ ์๋น์ค๊ฐ ์๊ฒผ๋ค([link](https://www.forbes.com/sites/dereksaul/2023/01/10/microsoft-reportedly-closing-in-on-10-billion-investment-into-chatgpt-creator-openai/?sh=5bb729fa3204)). ๋ง์ดํฌ๋ก์ํํธ๊ฐ Open AI ์ธ์ํจ์ ๋ฐ๋ผ AWS, GCP, Azure์ market share๋ Azure์ ํ๋ณด์ ์ํด ๋ฌ๋ผ์ง ์ ์์ ๊ฒ์ด๋ค. ํ๊ตญ์์ ์ฃผ๋ก ์ฐ์ด๋ AWS์ GCP ์ฌ์ด์ Azure ์ฌ์ฉ์๊ฐ ๋ ์ ์๋ค. ๋, Bing์๊ฒ ์ ์ฉ์ด ๋  ChatGPT๋ฅผ ํตํด Bing์ ์ฌ์ฉ๋์ด ๋ ์ ์์ ๊ฒ์ด๋ผ Google search engine์ market share๋ ์ค ์ ์๋ค. 
<div id="all-search_engine-ww-monthly-202201-202301"></div><!-- You may change the values of width and height above to resize the chart  width="600" height="400" style="width:600px; height: 400px;"--><p><i>Source: <a href="https://gs.statcounter.com/search-engine-market-share">StatCounter Global Stats - Search Engine Market Share</a></i></p><script type="text/javascript" src="https://www.statcounter.com/js/fusioncharts.js"></script><script type="text/javascript" src="https://gs.statcounter.com/chart.php?all-search_engine-ww-monthly-202201-202301&chartWidth=600"></script>

- Multi-modal learning AI๋ฅผ ํตํด ์์ผ๋ก text์ ํ ๋๋ฉ์ธ ํ์ต๋ณด๋ค text-to-image (DALL-E), text-to-video ๋ฑ์ ๋ฉํฐ ๋๋ฉ์ธ generative AI๊ฐ ๋ ํฅํํ  ์๋ ์์ ๊ฒ์ด๋ค. ChatGPT๋ ์ฑ๋ด์ ํํ๋ก ํน์ํ๊ฒ ํ๋ จ๋ ๋ชจ๋ธ์ธ๋ฐ, ๊ทธ ์ดํ๋ก CLIP์ด๋ ๊ธฐ์ ์ ํตํด ์ด๋ฏธ ๋ง๋ค์ด์ง text-to-image ๋ชจ๋ธ์ธ DALL-E 2([link](https://openai.com/dall-e-2/))๋ฅผ ๋ฅ๊ฐํ๋ ๋ ์ฌ์ธํ๊ณ  semanticํ ๊ทธ๋ฆผ์ ์์ฑํ๋ DALL-E 3๋, 2d๋ฅผ ๋์ด์๋ 3d ์ด๋ฏธ์ง ์์ฑ์ด๋, ๋น๋์ค ์์ฑ์ ํ๋ ๋จ๊ณ๊น์ง ๊ฐ ์ ์๋ค.

- ๋ํ, ์ต๊ทผ ๋๋๋๋ ๊ฒ์ OpenAI์์ ๊ทผ๋ฌดํ ๋ถ๋ค์ด ์ฐจ๋ฆฐ ์คํํธ์์ ์ฑ์ฅ์ธ์ด๋ค. 2021๋์ ์ธ์์ง Anthropic์ Claude๋ ์ฑ๋ด์ ๋ฐ๋ก ๋ง๋ค์ด์ **2022๋ ๋ง์ Google์ด 300 million USD๋ฅผ ์ฌ๊ธฐ์ ํฌ์**ํ๋ค([link](https://www.theverge.com/2023/2/3/23584540/google-anthropic-investment-300-million-openai-chatgpt-rival-claude)). ChatGPT๋ ์ธ๊ฐ์ ํผ๋๋ฐฑ์ ์์ฉํ ๊ฐํํ์ต์ ์ผ์ข์ธ reinforcement learning from human feedback (RLHF)์ ๋ฐ๋๊ณ , Anthropic์ Constitution AI๋ ๋ชจ๋ธ์ ์จ์ fine-tuned๋ ์์ํ์ ๋ํด ์ธ๊ฐ์ด ์๋ ์ปดํจํฐ๊ฐ ๊ฐํํ์ต์ ์งํํ๋๋ก ํ ์ฐจ์ด๊ฐ ์๋ค([link](https://scale.com/blog/chatgpt-vs-claude)). Anthropic ์ด์ธ์๋ ๋ค์์ ํ์ ์คํํธ์์ด ์๊ฒจ๋ ์ด์  ์๋ ๊ทธ๋ฆผ๊ณผ ๊ฐ์ด ํ์ดํ ๋งํผ์์ ์ด์ด OpenAI ๋งํผ์๋ ๋ช์นญ์ด ์๊ฒจ๋ฌ๋ค.

![openai-mafia](./assets/img/openai-mafia.jpg)
*Analytics India Magazine. (2023). OpenAI Mafia. https://analyticsindiamagazine.substack.com/p/openai-mafia*

- 2023๋ ์์ธ๋ ์ด๊ต๊ตฌ ๊ต์๋์ Supertone (Mnet, SBS ๋ฑ์์ ์ฃฝ์ ๊ฐ์๊ฐ ํ์ํด ์ต์ ๊ณก์ ์ปค๋ฒํจ)์ ์ธ์ํ ํ์ด๋ธ์ฒ๋ผ ์ต์  ๋ฆฌ์์น์ ๊ด์ฌ์ด ์๋ ์คํํธ์์ด ๊ฒฝ์๋ ฅ์ด ์๊ณ  IPํ๋ณด์ ์ ๋ฆฌํ  ๊ฒ์ด๋ค. ์ง๋ **2023๋ 1์ 31์ผ ํ์ด๋ธ๊ฐ Supertone์ 490์ต์์ ํฌ์ํด 56%์ ์ง๋ถ**์ ๋ฐ์ ๊ณผ๋ฐ์์ ์ง๋ถ์ ํ๋ณดํ๋ค([link](https://www.sbiz.news/news/articleView.html?idxno=22377)). Supertone๊ณผ ๊ฐ์ ๊ฒฝ์ฐ์๋ ๊ธ์ด์ด ๋ณธ์ธ์ ์ ์ฐ๊ตฌ์ค์ด์๊ณ , ๊ต์๋์ ์์์ ๋ค์ ๋ฐ๋ก ์์ฑ ๋ฟ๋ง์ด ์๋๋ผ ์๋ฌด๋ฅผ ์์๋นํธ์ ๋ง์ถฐ ์์ฑํ๋ค๋ ์ง์ ์ฐ๊ตฌ๊ฐ ์๋ ๊ฐ ์ด๋ฃจ์ด์ก๋ค. ๋, ์ฐ๊ตฌ์ค ์์ ์คํํธ์์ผ๋ก ์์ธ๋ **์ ๋ณ๊ณค ๊ต์๋์ FriendliAI**([link](https://friendli.ai/))๊ฐ ์๋ค. PeriFlow๋ GPT-3์ ๊ฒฝ๋๋ ๋ฒ์  ์๋น์ค๋ฅผ ๋ง๋ค์ด ๋ฐฐํฌํ๊ณ  ์์ผ๋ฉฐ, ์ด๋ฅผ ํตํด Scatter Lab์ ์ด๋ฃจ๋ค ์ฑ๋ด์ด ์ํฌํธ ๋๊ณ  ์๋ค.

![hybe-supertone](./assets/img/hybe-supertone.jpg)

- ์ธ๊ณต์ง๋ฅ ์ปจํ์ธ  ์ชฝ์ voice.ai๋ฅผ ๋ณด๋ฉด ์ ํ๋ธ์ ์ผ์ธ ๋ก ์ผ๋ฐ์ธ์ด ์ผ๋ก  ๋จธ์คํฌ์ ๋น๋์ค๋ก ๋ค๋ฅธ ๋ชฉ์๋ฆฌ(๋ชจ๊ฐ ํ๋ฆฌ๋จผ, ์กฐ ๋ฐ์ด๋ , ์ค๋๋ฅ ํ์ดํธ ๋ฑ 50์ฌ ๊ฐ์ง)์ sync๋ฅผ ๋ง์ถ ์ ์๋ ์์๋ค์ ์ ์ ๋ค์ด ๊พธ์คํ ์ฒดํํด ๋ณผ ์ ์๊ฒ๋ ํ๋ค([link](https://youtube.com/shorts/S84CgeVCNO8?feature=share)). ๋ค๋ฅธ ๋น๋์ค์์๋ Roblox์ voice.ai๋ฅผ ํตํด ๋ชฉ์๋ฆฌ๋ฅผ ์ํ๋ ๋ฒ์ ์๋ ค์ค๋ค. ๊ฐ์ ํ๋ฆฌํฐ์ Core AI ๊ธฐ์ ์ด๋๋ผ๋ ๊ฐ์ข ์ฐฝ์์ ์ธ ์๋จ์ผ๋ก B2C, B2B ํ๋ณดํ๊ณ  ์์๋ฌธ์ด ์ ๋๊ฒ๋ ํ๋ ์คํํธ์๋ค์ด ChatGPT์ ๊ฐ์ ํญํ์  ์ธ๊ธฐ๋ฅผ ๋ ์ ์์ ๊ฒ์ด๋ค.

- ์์ ์ปจํ์ธ ์ ์ด์ด์ NVIDIA์ ๊ฐ์ ๊ฒฝ์ฐ์๋ ๋์ ์์ ์ ์์ฐ์ค๋ฝ๊ฒ ๋ณด์ ํด์ฃผ๋ ๊ธฐ์ (NVIDIA Broadcast)์ด ๊ฐ๋ฐ์ด ๋์๊ณ , 2023๋ ํ์ฌ 1.4๋ฒ์  ์๋น์ค ์ค์ด๋ค([link](https://www.nvidia.com/en-us/geforce/news/jan-2023-nvidia-broadcast-update/)). ์ด๋ฅผ ํตํด ์ฌ๋๋ค์ด ๋๋ณธ์ ์ฝ๊ณ  ์น์บ  ์์ ๋ฐํ๋ฅผ ํ  ๋, ๋๋ณธ์ ๋์ด ๊ฐ ์๊ฑฐ๋, ๋ค๋ฅธ ๊ณณ์ ๋์ด ํฅํด ์์ด๋ NVIDIA Broadcast๋ก ๋์ ์นด๋ฉ๋ผ๋ก ํฅํ  ์ ์๊ฒ๋ ๋ณด์ ํด ์ค๋ค. ์ด ๊ธฐ์ ์ ํตํด ํ์ฉํ  ์ ์๋ ์ํฉ๋ค์ ๊พธ์คํ ์์๋ค๋ก PRํด ์ฌ๋๋ค์ ๊ด์ฌ์ ๋ชจ์ ์ ์๋ค([link](https://www.youtube.com/watch?v=O50BkP16eZo)).

<video controls muted autoplay loop>
  <source src="./assets/img/nvidia-broadcast.mp4" type="video/mp4">
</video>

### ์ต์  ํซํ ๋ผ๋ฌธ๋ค์ ๋ํ ๋ด์ฉ์ ๋ค์์ฃผ DTW-2์ ํ์ธ๊ฐ๋ฅ

- ๋ผ๋ฌธ์ ๋ด๋ ๊ณณ ์ค์ ์ปจํผ๋ฐ์ค์ ์ ๋ ๋ฑ์ด ์๊ณ , IF๊ฐ ๋์์๋ก ๋ ๋ช์ฑ์ด ๋์ ๊ณณ์ด๋ผ ํ  ์ ์๋ค. ICLR, NIPS, ICML, AAAI, CVPR ๋ฑ์ด ์๋ค([link](https://scholar.google.es/citations?view_op=top_venues&hl=en&vq=eng_artificialintelligence)).

- ๋ผ๋ฌธ์ ์ ์ถํด์ accept๋๊ณ  ์ถํ๋  ๋ ๋ฐ๋ก ํซํด์ง๋ ๋ผ๋ฌธ์ด ์๋๊ฐ ํ๋ฉด, ํ์ฐธ ํ์ ์ ๋ชํด์ง๋ ๋ผ๋ฌธ๋ค๋ ์๋ค. ๋ณดํต์ ์ฐ์์์ ์ฐ์ด๊ธฐ ์ ์ ์ด๋ฏธ ์ฐ์ผ ๋ผ๋ฌธ ๊ธฐ์ ๋ค์ ์ ๋ชํด์ง๋ค<sub>(2014๋ ์ฒ์ ๋์๋ GAN์ 2020๋ ์ทจ์์ ํ  ๋์๋ ์ฌ๋ฌ ์คํํธ์์์ ์ธ ์ ์๋์ง ์ทจ์๊ณต๊ณ ์ ์ ์ํ๊ธฐ๋ ํ๋ค)</sub>.

<!---
Week 2
- About all the licenses that could be included in open source software (Apache 2.0, etc.).
- ํํฌ ๊ธฐ์๋ค์ ๋ํ ๋ฏธ๊ตญ์ ์ต์  valuation ๋ฐฉ๋ฒ๋ค
- Midjourney
- Microsoft Teams๊ฐ Notion๋ณด๋ค ์ธ๊ธฐ๊ฐ ๋ง์์ง ์ด์ ๋ ์ด๋ฏธ ์ ์ ํ๊ณ  ์๋ Windows์ distribution ๋๋ฌธ.
- ๊ตฌ๊ธ์ด ๋ฐ๋๋ฅผ ์ถ์
- ๋ฐ๋์ ์ค์
- OpenAI's business structure (not feature, not product)
- ๋ฉํ๋ฒ์ค์์ ์์ ๋ MS
- Google์ AI Test Kitchen์ ํตํด์ waitlist์ ๋ฑ๋กํ ๋ค์ LaMDA ์คํํด ๋ณผ ์ ์์.
- ์ธ์๋ AI ์คํํธ์์ ๋ํ ์กฐ์ฌ - Bedrock Data acquired by Formstack, AuthAir acquired by LogMeIn, Carbon Black acquired by VMWare, Connotate acquired by import.io, edgewise networks acquired by zscaler
- ์ธ์๋ฅผ ์ํ๋ ์ธ๊ตญ๊ธฐ์ ๋ฐ ํ๊ตญ๊ธฐ์
- ๋ณธ๋๋ ํ๋ฆฌ ์คํํธ์ BeReal๊ณผ ๋น์ทํ๋ค https://www.linkedin.com/posts/amyrlewin_socialmedia-frenchtech-genz-activity-7029033711861944320-0M9g?utm_source=share&utm_medium=member_android
-->
