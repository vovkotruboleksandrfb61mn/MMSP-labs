# Математичне моделювання систем і процесів — лабораторні роботи

Вовкотруб Олександр Віталійович, група ФБ-61мн
Навчально-науковий фізико-технічний інститут, кафедра інформаційної безпеки
КПІ ім. Ігоря Сікорського

Викладач: доц. Смирнов С. Варіант 3 в усіх роботах.

| № | Тема | Ноутбук | Звіт |
|---|------|---------|------|
| 1 | Засоби моделювання Python: фігури Лісажу, поліном Чебишева, годограф Михайлова, банкомат | [solution.ipynb](lab1/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/MMSP-labs/blob/main/lab1/solution.ipynb) | [PDF](lab1/LR1_ZasobyPython_Vovkotrub_FB-61mn.pdf) |
| 2 | Моделювання лінійних систем: стійкість, часові та частотні характеристики, канонічні форми | [solution.ipynb](lab2/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/MMSP-labs/blob/main/lab2/solution.ipynb) | [PDF](lab2/LR2_LiniyniSystemy_Vovkotrub_FB-61mn.pdf) |
| 3 | Мережі Петрі: граф досяжних розміток, P-інваріанти, обідаючі філософи | [solution.ipynb](lab3/solution.ipynb) · [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/vovkotruboleksandrfb61mn/MMSP-labs/blob/main/lab3/solution.ipynb) | [PDF](lab3/LR3_MerezhiPetri_Vovkotrub_FB-61mn.pdf) |

## Запуск

**У Colab** — відкрити ноутбук за кнопкою в таблиці й виконати
*Runtime → Run all*. Перша клітинка сама доставляє відсутні пакети (для ЛР3 —
ще й системний Graphviz), тож нічого готувати вручну не треба.

**Локально** (Python 3.13):

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook lab1/solution.ipynb   # або lab2/…, lab3/…
```

Для ЛР3 потрібен ще системний Graphviz — ним рендеряться мережі Петрі:

```bash
sudo dnf install graphviz     # або: sudo apt install graphviz
```

Кожен ноутбук самодостатній: код допоміжних модулів вбудовано в нього
окремими клітинками, а теки `assets/` і `data/` створюються поруч під час
виконання.
