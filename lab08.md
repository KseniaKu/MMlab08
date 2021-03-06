---
title: "Лабораторная работа №8"
author: "Кувшинова К.О. группа НФИ-02-19"
subtitle: "Модель конкуренции двух фирм"
output:
  word_document: default
  pdf_document: default
toc-title: Содержание
toc: yes
toc_depth: 2
lof: yes
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: yes
pdf-engine: lualatex
header-includes:
- \linepenalty=10
- \interlinepenalty=0
- \hyphenpenalty=50
- \exhyphenpenalty=50
- \binoppenalty=700
- \relpenalty=500
- \clubpenalty=150
- \widowpenalty=150
- \displaywidowpenalty=50
- \brokenpenalty=100
- \predisplaypenalty=10000
- \postdisplaypenalty=0
- \floatingpenalty = 20000
- \raggedbottom
- \usepackage{float}
- \floatplacement{figure}{H}
---


# Цель работы

Рассмотреть модель конкуренции двух фирм для двух случаев: без учета социально-психологического фактора и с ним.

# Задание работы

### Вариант 36

**Случай 1.** Рассмотрим две фирмы, производящие взаимозаменяемые товары одинакового качества и находящиеся в одной рыночной нише. Считаем, что в рамках нашей модели конкурентная борьба ведётся только рыночными методами. То есть, конкуренты могут влиять на противника путем изменения параметров своего производства: себестоимость, время цикла, но не могут прямо вмешиваться в ситуацию на рынке («назначать» цену или влиять на потребителей каким-либо иным способом.) Будем считать, что постоянные издержки пренебрежимо малы, и в модели учитывать не будем. В этом случае динамика изменения объемов продаж фирмы 1 и фирмы 2 описывается следующей системой уравнений:

$\frac{dM_1}{d\theta}=M_1-\frac{b}{c_1}M_1M_2-\frac{a_1}{c_1}M_1^2$ ,

$\frac{dM_2}{d\theta}=\frac{c_2}{c_1}M_2-\frac{b}{c_1}M_1M_2-\frac{a_2}{c_1}M_2^2$

где 
$a_1=\frac{p_{cr}}{\tau_1^2\widetilde p_1^2Nq}$ , 
$a_2=\frac{p_{cr}}{\tau_2^2\widetilde p_2^2Nq}$ ,
$b=\frac{p_{cr}}{\tau_1^2\widetilde p_1^2\tau_2^2\widetilde p_2^2Nq}$ ,
$c_1=\frac{p_{cr}-\widetilde p_1}{\tau_1\widetilde p_1}$ ,
$c_2=\frac{p_{cr}-\widetilde p_2}{\tau_2\widetilde p_2}$.

Также введена нормировка $t=c_1\theta$

**Случай 2.** Рассмотрим модель, когда, помимо экономического фактора влияния (изменение себестоимости, производственного цикла, использование кредита и т.п.), используются еще и социально-психологические факторы – формирование общественного предпочтения одного товара другому, не зависимо от их качества и цены. В этом случае взаимодействие двух фирм будет зависеть друг от друга, соответственно коэффициент перед $M_1M_2$ будет отличаться. Пусть в рамках рассматриваемой модели динамика изменения объемов продаж фирмы 1 и фирмы 2 описывается следующей системой уравнений:

$\frac{dM_1}{d\theta}=M_1-\frac{b}{c_1}M_1M_2-\frac{a_1}{c_1}M_1^2$ ,

$\frac{dM_2}{d\theta}=\frac{c_2}{c_1}M_2-(\frac{b}{c_1}+0.00063)M_1M_2-\frac{a_2}{c_1}M_2^2$

Для обоих случаев рассмотрим задачу со следующими начальными условиями: 

$M_0^1=3.7,M_0^2=2.8,$

$p_{cr}=27, N=37,q=1$

и параметрами:

$\tau_1=27, \tau_2=17,$

$\widetilde p_1=6.7$ , $\widetilde p_2=11.7$

***Замечание:*** значения $p_{cr}, \tilde p_{1,2}, N$ указаны в тысячах единиц, а значения $M_{1,2}$ указаны в млн. единиц.

***Обозначения:***

N – число потребителей производимого продукта.

$\tau$ – длительность производственного цикла

p – рыночная цена товара

$\tilde p$– себестоимость продукта, то есть переменные издержки на производство единицы продукции.

q – максимальная потребность одного человека в продукте в единицу времени

$\theta=\frac{t}{c_1}$- безразмерное время

1. Постройте графики изменения оборотных средств фирмы 1 и фирмы 2 без учета постоянных издержек и с веденной нормировкой для случая 1.
2. Постройте графики изменения оборотных средств фирмы 1 и фирмы 2 без учета постоянных издержек и с веденной нормировкой для случая 2.


# Теоретичсекое введение

***Случай 1***
Рассмотрим две фирмы, производящие взаимозаменяемые товары
одинакового качества и находящиеся в одной рыночной нише. Последнее означает, что у потребителей в этой нише нет априорных предпочтений, и они приобретут тот или иной товар, не обращая внимания на знак фирмы.

В этом случае, на рынке устанавливается единая цена, которая определяется балансом суммарного предложения и спроса. Иными словами, в рамках нашей модели конкурентная борьба ведётся только рыночными методами. То есть, конкуренты могут влиять на противника путем изменения параметров своего производства: себестоимость, время цикла, но не могут прямо вмешиваться в ситуацию на рынке («назначать» цену или влиять на потребителей какимлибо иным способом.)

$\frac{dM_1}{d\theta}=M_1-\frac{b}{c_1}M_1M_2-\frac{a_1}{c_1}M_1^2$ ,

$\frac{dM_2}{d\theta}=\frac{c_2}{c_1}M_2-\frac{b}{c_1}M_1M_2-\frac{a_2}{c_1}M_2^2$

где 
$a_1=\frac{p_{cr}}{\tau_1^2\widetilde p_1^2Nq}$ , 
$a_2=\frac{p_{cr}}{\tau_2^2\widetilde p_2^2Nq}$ ,
$b=\frac{p_{cr}}{\tau_1^2\widetilde p_1^2\tau_2^2\widetilde p_2^2Nq}$ ,
$c_1=\frac{p_{cr}-\widetilde p_1}{\tau_1\widetilde p_1}$ ,
$c_2=\frac{p_{cr}-\widetilde p_2}{\tau_2\widetilde p_2}$.

Также введена нормировка $t=c_1\theta$

Рост оборотных средств предприятий идет независимо друг от друга. В математической модели этот факт отражается в
коэффициенте, стоящим перед членом
$M_1M_2$ : в рассматриваемой задаче он одинаковый в обоих уравнениях $(\frac{b}{c_1})$. Это было обозначено в условиях задачи. Каждая фирма достигает свое максимальное значение объема продаж и остается на рынке с этим значением, то есть каждая фирма захватывает свою часть рынка потребителей, которая не изменяется.

***Случай 2***

Рассмотрим модель, когда, помимо экономического фактора влияния (изменение себестоимости, производственного цикла, использование кредита и т.п.), используются еще и социально-психологические факторы – формирование общественного предпочтения одного товара другому, не зависимо от их качества и цены. В этом случае взаимодействие двух фирм будет зависеть друг от друга,
соответственно коэффициент перед $M_1M_2$ будет отличаться:

$\frac{dM_1}{d\theta}=M_1-\frac{b}{c_1}M_1M_2-\frac{a_1}{c_1}M_1^2$ ,

$\frac{dM_2}{d\theta}=\frac{c_2}{c_1}M_2-(\frac{b}{c_1}+l)M_1M_2-\frac{a_2}{c_1}M_2^2$

где l - коэффициент социально-психологического фактора

Первая фирма, несмотря на начальный рост, достигнув своего максимального объема продаж, начнет нести убытки и, в итоге, претерпит банкротство. Динамика роста объемов оборотных средств второй фирмы остается без изменения: достигнув максимального значения, остается на этом
уровне. [^1]



# Выполнение лабораторной работы

### Решение

***Случай 1***

$\frac{dM_1}{d\theta}=M_1-\frac{b}{c_1}M_1M_2-\frac{a_1}{c_1}M_1^2$ ,

$\frac{dM_2}{d\theta}=\frac{c_2}{c_1}M_2-\frac{b}{c_1}M_1M_2-\frac{a_2}{c_1}M_2^2$

где 
$a_1=\frac{p_{cr}}{\tau_1^2\widetilde p_1^2Nq}$ , 
$a_2=\frac{p_{cr}}{\tau_2^2\widetilde p_2^2Nq}$ ,
$b=\frac{p_{cr}}{\tau_1^2\widetilde p_1^2\tau_2^2\widetilde p_2^2Nq}$ ,
$c_1=\frac{p_{cr}-\widetilde p_1}{\tau_1\widetilde p_1}$ ,
$c_2=\frac{p_{cr}-\widetilde p_2}{\tau_2\widetilde p_2}$.

Также введена нормировка $t=c_1\theta$

Код программы в OpenModelica (для обоих случаев) (@fig:001):

![Код программы](код.png){#fig:001 width=100%}

График изменения оборотных средств для фирмы 1 и фирмы 2 (@fig:002):

![График изменения оборотных средств фирмы 1 и фирмы 2  для случая 1 ](график1.png){#fig:002 width=100%}

***Случай 2***

$\frac{dM_1}{d\theta}=M_1-\frac{b}{c_1}M_1M_2-\frac{a_1}{c_1}M_1^2$ ,

$\frac{dM_2}{d\theta}=\frac{c_2}{c_1}M_2-(\frac{b}{c_1}+0.00063)M_1M_2-\frac{a_2}{c_1}M_2^2$

График изменения оборотных средств фирмы 1 и фирмы 2  с учетом социально-психологического фактора (@fig:003):

![График изменения оборотных средств фирмы 1 и фирмы 2  с учетом социально-психологического фактора для случая 2 ](график2.png){#fig:003 width=100%}


# Вывод

В ходе выполнения работы мы рассмотрели и построили модель конкуренции двух фирм для двух случаев: без учета социально-психологического фактора и с ним.


# Библиография

   1.  Кулябов, Д.С. Модель конкуренции двух фирм  [Текст] / Д.С.Кулябов. - Москва: - 7 с. [^1]: Кулябов, Д.С. Модель конкуренции двух фирм.