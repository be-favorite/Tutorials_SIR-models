# SIR 모형을 이용한 전염병 유행 모델링

* How can we forecast COVID-19?: https://robjhyndman.com/hyndsight/forecasting-covid19/
* SIR 모형 소개 및 R을 이용한 튜토리얼:

## Introduction
전염병 유행의 모형화에 초석이 되는 대표적 모형 SIR(Susceptible-Infected-Recovered) 모형에 대해 소개합니다. COVID-19로 인한 팬데믹 상황의 지속으로 COVID-19 일별 확진자에 대한 예측 모델링에 관심이 있는 분들이 많을거라 생각되는데, 전염병 확진자와 관련한 예측 모델링을 확진자의 수가 단순히 시간 순서로 관측된다고 하여 시계열 모형으로 모델링을 하는 행위는 지양해야 합니다. 그 이유가 궁금하다면 상기 링크(How can we forecast COVID-19?)를 참고해주시기 바랍니다. 시계열 분석의 대가라 할 수 있는 Hyndman이 개인 블로그에 기술한 글입니다. 해당 글의 결론은 어쨌든 전염병 유행에 따른 확진자 수 등에 관한 모델링에는 SIR 모형과 같이 전염병과 관련한 예측(e.g. 확진자 수)을 목적으로 만들어진 수학적 모형으로 수행하는 것이 훨씬 더 좋은 예측 성능을 낼 수 있다는 것입니다. 요즘 COVID-19 백신 도입에 따른 팬데믹 상황에 대한 앞으로의 여러가지 시나리오(e.g. 사회적 거리두기, 백신 효능에 따른 확진자 수 예측)에 대한 연구가 활발하게 진행 중인데, [The Lancet Infectious Diseases](https://www.thelancet.com/journals/laninf/home)을 통해 관련 연구(e.g. [Sandmann, Frank & Davies, Nicholas & Vassall, Anna & Edmunds, W & Jit, Mark. (2020)](https://www.sciencedirect.com/science/article/pii/S1473309921000797))를 살펴보면 이러한 전염병 유행의 여러 시나리오에 관한 예측 모델링에는 SIR 모형을 근간으로 하는 좀 더 복잡한 수학적 모형(여러가지 시나리오를 가정하기 위한)들이 사용되고 있음(e.g. SEIR models)을 확인할 수 있습니다. 해당 레포에 정리한 글(SIR 모형 소개 및 R을 이용한 튜토리얼)을 잘 이해한다면, 좀 더 복잡한 형태를 띠는 전염병 모형들의 이해에 큰 도움이 될 거라 생각합니다.😊

<br>

<div align=center>
 
[![Github Badge](http://img.shields.io/badge/-Github%20profile-black?style=flat-square&logo=github&link=https://github.com/be-favorite)](https://github.com/be-favorite) 
[![Tistory badge](https://img.shields.io/badge/-Tistory%20blog-yellow?style=flat-square&logo=Blogger&link=https://be-favorite.tistory.com/)](https://be-favorite.tistory.com/) 
[![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/taemo-bang-8b9999184/)](https://www.linkedin.com/in/taemo-bang-8b9999184/) 
[![Instagram Badge](https://img.shields.io/badge/-Instagram-dd2a7b?style=flat-square&logo=instagram&logoColor=white&link=https://www.instagram.com/qkdxoah/)](https://www.instagram.com/qkdxoah/) 

</div>
