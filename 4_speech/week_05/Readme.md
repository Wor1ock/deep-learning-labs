## Материалы модуля 5


### Распознавание речи.
В этом модуле вы изучите ключевые архитектуры распознавания речи и на практике поработаете с датасетами и моделями.

### Лекция

<div style="display: flex; gap: 8px; align-items: baseline; white-space: nowrap; line-height: 1.2; margin-bottom: 16px;">
  <span>Запись лекции &laquo;Распознавание речи&raquo; доступна на</span>
  <a href="https://youtu.be/Sen3B5ROm0I" target="_blank" rel="noopener" aria-label="Watch on YouTube" style="text-decoration: none;">
    <img src="https://cdn.simpleicons.org/youtube" alt="YouTube" width="20" style="vertical-align: bottom;"> YouTube
  </a>
  <span>и</span>
  <a href="https://vkvideo.ru/video-155161349_456239325" target="_blank" rel="noopener" aria-label="Watch on VK" style="text-decoration: none;">
    <img src="https://cdn.simpleicons.org/vk" alt="VK" width="20" style="vertical-align: bottom;"> VK Видео
  </a>
</div>

На этой лекции вы познакомитесь с ключевыми концепциями распознавания речи. Мы разберем постановку задачи и метрики оценки моделей, поговорим про проблему выравнивания аудио и текста с помощью CTC-лосса, а также подробно разберём его формулу. Изучим архитектуры акустических энкодеров, поговорим про тренды их изменения с течением времени. Также обсудим модели основанные на Encoder-Decoder и RNN-Transducer архитектурах, сравним их с CTC подходом, разберём их сильные и слабые стороны.

Занятие ведёт Георгий Апарин


### Семинар

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DeepLearningSchool/Speech/blob/main/week_05_speech_asr/Practice/asr-sem-1.ipynb)

<div style="display: flex; gap: 8px; align-items: baseline; white-space: nowrap; line-height: 1.2; margin-bottom: 16px;">
  <span>Запись семинара &laquo;Распознавание речи&raquo; доступна на</span>
  <a href="https://youtu.be/Amq-DrjUXGA" target="_blank" rel="noopener" aria-label="Watch on YouTube" style="text-decoration: none;">
    <img src="https://cdn.simpleicons.org/youtube" alt="YouTube" width="20" style="vertical-align: bottom;"> YouTube
  </a>
  <span>и</span>
  <a href="https://vk.com/video-155161349_456239326" target="_blank" rel="noopener" aria-label="Watch on VK" style="text-decoration: none;">
    <img src="https://cdn.simpleicons.org/vk" alt="VK" width="20" style="vertical-align: bottom;"> VK Видео
  </a>
</div>

На семинаре мы детально разберём практические аспекты работы с системами автоматического распознавания речи. Поработаем с реальным датасетом LibriSpeech, вы научитесь вычислять метрику WER с подсчётом замен, удалений и вставок. Также реализуем расчет CTC-лосса на практике, протестируем его на различных сценариях. Поработаем с предобученной Conformer-CTC моделью из библиотеки NeMo, провалидируем её на наших данных. Сравним скорость инференса оригинальной модели Whisper с оптимизированной faster-whisper. Мы также поработаем с предобученной RNN-Transducer моделью, разберём её компоненты и алгоритм их инференса.


Занятие ведёт  Георгий Апарин


