
## Материалы модуля 6


### Распознавание речи. Часть 2.
В этом модуле вы узнаете, как методы адаптации вроде shallow fusion и hotwords помогают исправлять лингвистические ошибки ASR моделей.


### Лекция
<div style="display: flex; gap: 8px; align-items: baseline; white-space: nowrap; line-height: 1.2; margin-bottom: 16px;">
  <span>Запись лекции &laquo;Распознавание речи, часть 2&raquo; доступна на</span>
  <a href="https://youtu.be/jkUyjapgXgs" target="_blank" rel="noopener" aria-label="Watch on YouTube" style="text-decoration: none;">
    <img src="https://cdn.simpleicons.org/youtube" alt="YouTube" width="20" style="vertical-align: bottom;"> YouTube
  </a>
  <span>и</span>
  <a href="https://vk.com/video-155161349_456239329" target="_blank" rel="noopener" aria-label="Watch on VK" style="text-decoration: none;">
    <img src="https://cdn.simpleicons.org/vk" alt="VK" width="20" style="vertical-align: bottom;"> VK Видео
  </a>
</div>


На лекции мы обсудим какие бывают вне-доменные данные в задаче распознавания речи, разделим акустическую и лингвистическую природу ошибок. Укажем какие есть методы решения лингвистических ошибок, как считается OracleWER и как ставится задача реранкинга гипотез. Адаптация внутри лучевого поиска - основная тема лекции, разберём формулу shallow fusion, которая добавляет в скор дополнительной лингвистической модели по ходу формирования луча. Также поговорим про то какие используются модели, их преимущества и недостатки, затронем тему горячих слов и в конце сформируем итоговый пайплайн адаптации



### Семинар

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DeepLearningSchool/Speech/blob/main/week_06_speech_asr_2/Practice/asr_sem_2.ipynb)

<div style="display: flex; gap: 8px; align-items: baseline; white-space: nowrap; line-height: 1.2; margin-bottom: 16px;">
  <span>Запись семинара &laquo;Распознавание речи&raquo; доступна на</span>
  <a href="https://youtu.be/GWfB_lX_L7k" target="_blank" rel="noopener" aria-label="Watch on YouTube" style="text-decoration: none;">
    <img src="https://cdn.simpleicons.org/youtube" alt="YouTube" width="20" style="vertical-align: bottom;"> YouTube
  </a>
  <span>и</span>
  <a href="https://vk.com/video-155161349_456239330" target="_blank" rel="noopener" aria-label="Watch on VK" style="text-decoration: none;">
    <img src="https://cdn.simpleicons.org/vk" alt="VK" width="20" style="vertical-align: bottom;"> VK Видео
  </a>
</div>

На семинаре мы разберём практическое применение методов адаптации к системе распознавания речи. Работа будет построена вокруг аудио датасета, в транскрипциях которого много медицинских терминов. Вы научитесь использовать библиотеку pyctcdecode для лучевого поиска лучшей гипотезы. Также поработаем с Oracle-WER и горячими словами (hotwords). Детально посмотрим на то как использовать pyctcdecode с shallow fusion и дополнительной лингвистической моделью, с помощью библиотеки kenlm обучим внутри-доменную лингвистическую модель для медицинских текстов и применим её для улучшения качества распознавания на датасете.


### Домашнее задание

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DeepLearningSchool/Speech/blob/main/week_06_speech_asr_2/Homework/asr_hw.ipynb)

В домашнем задании вам предстоит реализовать архитектуру Conformer по статье, написать свой класс CTC-loss'а на torch и обучить ваш Conformer с вашим лоссов на датасете LibriSpeech. Во второй части домашнего задания вам нужно будет адаптировать вашу модель к аудио из медицинского домена, реализовать shallow fusion подход с N-Gram и с RNN-LM моделями. Результатом вашей работы станет пайплайн с обученной вами моделью, которая сохранит высокое качество распознавания на LibriSpeech и достигнет достаточного качества на данных медицинского домена.