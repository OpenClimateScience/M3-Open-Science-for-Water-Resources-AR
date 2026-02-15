<div dir="rtl" align="right">

<p align="right">
<a href="https://doi.org/10.5281/zenodo.16896539">
<img src="https://zenodo.org/badge/867199973.svg" alt="DOI">
</a>
</p>

<h1 align="right">
الوحدة M3: العلم المفتوح للموارد المائية
</h1>

<p align="right">
<span dir="ltr">M3: Open Science for Water Resources</span>
</p>

</div>


> ما الأدوات ومجموعات البيانات المتاحة لقياس كمية المياه وتوفرها؟

تركّز الوحدة الثالثة من منهج  
<a href="https://openclimatescience.github.io/curriculum" dir="ltr">Open Climate Science Curriculum</a>  
على كيفية البدء في مشروع علمي حاسوبي قابل لإعادة الإنتاج، باستخدام الموارد المائية كمثال موضوعي.

## في نهاية هذه الوحدة، ينبغي أن تكون قادرًا على

- وصف التدفقات والمخازن الرئيسية في الدورة الهيدرولوجية الأرضية.
- معرفة أماكن الوصول إلى بيانات الاستشعار عن بُعد أو النماذج المتعلقة بانحرافات تخزين المياه، والنتح–التبخر، ورطوبة التربة.
- حساب ميزانية مائية.

---
<div dir="rtl">

## المحتويات

1. [إنشاء بيئة برمجية بحثية](https://github.com/OpenClimateScience/M3-Open-Science-for-Water-Resources/blob/main/notebooks/01_Creating_a_Research_Software_Environment.ipynb)
2. [تحليل مكعب بيانات الهطول العالمي](https://github.com/OpenClimateScience/M3-Open-Science-for-Water-Resources/blob/main/notebooks/02_Analyzing_a_Global_Precipitation_Data_Cube.ipynb)
3. [تتبّع التغييرات في الشيفرة البحثية](https://github.com/OpenClimateScience/M3-Open-Science-for-Water-Resources/blob/main/notebooks/03_Tracking_Changes_to_Research_Code.ipynb)
4. [إنشاء ميزانية مائية على مستوى الحوض](https://github.com/OpenClimateScience/M3-Open-Science-for-Water-Resources/blob/main/notebooks/04_Creating_a_Basin-Scale_Water_Budget.ipynb)
5. [توثيق سير عمل الميزانية المائية](https://github.com/OpenClimateScience/M3-Open-Science-for-Water-Resources/blob/main/notebooks/05_Documenting_our_Water_Budget_Workflow.ipynb)

</div>


## البدء

راجع دليل التثبيت هنا:  
<a href="https://github.com/OpenClimateScience/M1-Open-Climate-Data/blob/main/HOW_TO_INSTALL.md" dir="ltr">HOW_TO_INSTALL.md</a>

لتشغيل الدفاتر، يمكنك استخدام <span dir="ltr">GitHub Codespaces</span> أو <span dir="ltr">VSCode Dev Container</span>. بعد تشغيل البيئة، نفّذ:

```sh
# Create your own password when prompted
jupyter server password

# Then, launch Jupyter Notebook; enter your password when prompted
jupyter notebook
```

## تثبيت مكتبات Python المطلوبة

```sh
pip install xarray netcdf4 dask
```

## تنزيل البيانات المطلوبة

<a href="https://doi.org/10.5281/zenodo.16896169" dir="ltr">https://doi.org/10.5281/zenodo.16896169</a>

---

## نواتج التعلم

تغطي هذه الوحدة الكفاءات الأساسية التالية في علم البيانات الحاسوبي:

- اختيار أسماء ملفات ذات معنى (<span dir="ltr">CC1.3</span>)
- توثيق العلاقات بين الشيفرة والنتائج والبيانات الوصفية (<span dir="ltr">CC1.5</span>)
- استخدام مدير حزم لإدارة الاعتمادات البرمجية (<span dir="ltr">CC1.10</span>)
- فهم المصفوفات متعددة الأبعاد (<span dir="ltr">CC2.3</span>)
- توسيع نطاق سير العمل الحاسوبي (<span dir="ltr">CC2.6</span>)
- اختيار أسماء متغيرات واضحة ومعبّرة (<span dir="ltr">CC3.8</span>)
- فهم إصدارات البرمجيات وإدارتها (<span dir="ltr">CC4.4</span>)
- استخدام عبارات <span dir="ltr">assert</span> للتحقق من الفرضيات أثناء التنفيذ (<span dir="ltr">CC4.7</span>)
- كتابة دوال قصيرة وبسيطة دون تأثيرات جانبية (<span dir="ltr">CC4.9</span>)

**بالإضافة إلى ذلك، سيتعلم المتدربون كيفية:**

- تثبيت وإدارة حزم <span dir="ltr">Python</span>
- دمج عدة ملفات <span dir="ltr">HDF</span> في كائن <span dir="ltr">xarray.Dataset</span>
- اقتطاع بيانات <span dir="ltr">xarray</span> باستخدام ملف <span dir="ltr">ESRI Shapefile</span>
- قصّ وإعادة إسقاط بيانات الراستر (<span dir="ltr">raster</span>) باستخدام <span dir="ltr">Shapefile</span>
- حساب ميزانية مائية باستخدام الهطول والنتح–التبخر والجريان السطحي
- استخدام <span dir="ltr">Git</span> و<span dir="ltr">GitHub</span> لتتبع التغييرات ونسخ الشيفرة احتياطيًا

---

## مجموعات البيانات المناخية المستخدمة

- بيانات الهطول الشهرية من <a href="https://dx.doi.org/10.5067/GPM/IMERG/3B-MONTH/07" dir="ltr">NASA IMERG-Final</a>
- بيانات النتح–التبخر السنوية من <a href="https://lpdaac.usgs.gov/products/mod16a2v061/" dir="ltr">NASA MODIS MOD16</a>
- انحرافات تخزين المياه الأرضية من <a href="https://podaac.jpl.nasa.gov/dataset/TELLUS_GRAC-GRFO_MASCON_CRI_GRID_RL06.1_V3" dir="ltr">NASA GRACE وGRACE-FO</a>
- بيانات الجريان السطحي من <a href="https://doi.org/10.1038/s41597-020-00583-2" dir="ltr">HYSETS</a>

---

## شكر وتقدير

أُتيح تطوير هذا المنهج بفضل منحة من برنامج <span dir="ltr">NASA Transition to Open Science (TOPS)</span> للتدريب  
(<span dir="ltr">80NSSC23K0864</span>)، ضمن برنامج <a href="https://nasa.github.io/Transform-to-Open-Science/" dir="ltr">NASA TOPS</a>.

</div>
