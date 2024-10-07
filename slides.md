---
theme: default
background: https://cover.sli.dev
title: Cloud Carbon Footprint
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
transition: slide-left
mdc: true
export:
  format: pdf
  timeout: 30000
  dark: true
selectable: true
colorSchema: dark  
favicon: 'https://www.zatsit.fr/wp-content/uploads/2024/02/SIGLE-ZATSIT-BLEU-1.svg'
fonts:
  sans: Poppins
  serif: Poppins
  mono: Fira Code
---

# Cloud Carbon Footprint 
 Cloud Nord 2024

 <span style="color:#ff9900;font-size:45px">Emmanuel Péru - **zatsit**</span>


---
layout: default
---
# <span style="color:#ff9900">Who Am I ?</span>

<div grid="~ cols-2 gap-4">
<div>

🛠 <span style="color:#ff9900">**CTO chez zatsit** </span>

- Engager notre **expertise numérique** au service de l'**impact** des entreprises, en créant un écosystème **durable**, **partenarial** et **positif**

🎨 <span style="color:#ff9900">**Architecte Solutions** </span>
- Travailler en équipe pour résoudre des problèmes qu'on aurait jamais eu si on travaillait seul 

🤹 <span style="color:#ff9900">**Meetup Flutter Lille**</span>
- Co-organisateur des meetups pour développeur mobile, mais pas que !

</div>
<div>
<img  src="/images/eperu_x_profile.avif" alt="Description de l'image" width="400" height="400" style="display: block; margin: auto;"/>

<img  src="/images/eperu_linkedin_profile.avif" alt="Description de l'image" width="400" height="400" style="display: block; margin: auto;"/>

</div>
</div>
<!--  Retrouvez-moi sur les réseaux : https://www.linkedin.com/in/emmanuel-peru-10111274/ et https://x.com/EmmanuelPeru -->
---
layout: default
---
# <span style="color:#ff9900">What is zatsit ?</span>

🎂 NéoEsn qui a fêté ses 1 an

🕸️ Un réseau de 30 personnes passionnées et passionnantes

💻 Des sites web pour montrer et démontrer

🫴 L'envie de bien faire et d'être impactant

<img  src="/images/zatsit_sites.avif" alt="Description de l'image" width="500" height="500" style="display: block; margin: auto;"/> 

<!-- 4 vitrines éco conçues

  -->

---
layout: default
---

# <span style="color:#ff9900">À propos de la forme de ces slides</span>


### J'ai tenté une présentation différente pour changer

<br>

<div class="w-60 relative">
  <div class="relative w-40 h-40">
    <img
      v-motion
      :initial="{ x: 800, y: -100, scale: 1, rotate: -50 }"
      :enter="final"
      class="absolute inset-0"
      src="https://www.zatsit.fr/wp-content/uploads/2024/02/SIGLE-ZATSIT-BLEU-1.svg"
      alt=""
    /> 
    <img
      v-motion
      :initial="{ x: 600, y: 400, scale: 2, rotate: 100 }"
      :enter="final"
      class="absolute inset-0"
      src="https://avatars.githubusercontent.com/u/157115254?s=200&v=4"
      alt=""
    />
  </div>
  <div
    class="text-5xl absolute top-14 left-40 text-[#2B90B6] -z-1"
    v-motion
    :initial="{ x: -80, opacity: 0}"
    :enter="{ x: 0, opacity: 1, transition: { delay: 2000, duration: 1000 } }">    5Mo</div>
</div>
<script setup lang="ts">
const final = {
  x: 0,
  y: 0,
  rotate: 0,
  scale: 1,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
</script>

<div
  v-motion
  :initial="{ x:35, y: 30, opacity: 0}"
  :enter="{ y: 0, opacity: 1, transition: { delay: 3500 } }">
</div>


---
layout: two-cols
layoutClass: gap-16
---

# <span style="color:#ff9900">Au programme</span>

En <span v-mark.red="3"><code>20</code> minutes</span>

On va essayer de se sensibiliser 

<span v-mark.circle.orange="4">à l'empreinte de nos nuages</span>


::right::

<Toc v-click minDepth="1" maxDepth="2"></Toc>
<!-- CLIQUER pour les animations -->

---
layout: image-right
image: images/no_cloud.jpg
---

# Le cloud est une commodité ! 
<span style="color:#ff9900">
Imaginez qu'en quelques clics, on créé des ressources à l'autre bout de la terre, <b>PRESQUE</b> trop facilement ! 
</span>

Pour pas cher et sans grandes contraintes : 
- ça ne chauffe pas
- ça ne fait pas de bruit
- ça ne prend pas de place

<!-- Par CLI, Par Terraform, via la console -->
---
level: 2
layout: image-right
image: images/datacenter.webp
---

# Un nuage très dense
<span style="color:#ff9900">
Selon le cabinet Synergy Research :
</span>

- le nombre de datacenters exploités par les géants de l’internet et du cloud a dépassé <span style="color:#ff9900">**la barre des 1000**</span> au début de 2024.
- Et ce parc devrait <span style="color:#ff9900">**doubler**</span> dans les quatre années à venir, tiré par l’explosion des usages de l’IA.

- On nous annonçait la <span style="color:#ff9900">neutralité carbone</span>, mais l'IA est venue augmenter les besoins ! 

<span style="color:#ff9900">
Selon le département de l’énergie (EIA):
</span>

- la consommation d’énergie liée aux centres de données va plus que <span style="color:#ff9900">doubler</span> aux États-Unis d’ici 2030 pour consommer environ 9 % de toute l’électricité du pays.

<!-- On pourrait citer encore d'autres exemples avec OpenAI dont l'empreinte en eau et en électricité a été mesuré et est énorme -->

---
level: 2
layout: image-left
image: images/nuclear.avif
---

# <span style="color:#ff9900">On a plus de pétrole, mais on a des idées</span>

<br>
Microsoft a signé un accord d’achat d’électricité d’une durée de 20 ans avec la société Constellation, qui repose sur le <span style="color:#ff9900">redémarrage de la centrale nucléaire</span> de Three Mile Island en Pennsylvanie.

Oracle a sécurisé les permis pour construire <span style="color:#ff9900">trois petits réacteurs modulaires</span>. Avec ces derniers, la firme compte alimenter des data centers, pour notamment faire tourner des GPU Nvidia pour faire progresser l'IA.
<!-- Crédit photo : US Office of Nuclear Energy -->

---
layout: default
---

# <span style="color:#ff9900">La Green Software Foundation</span>

  - > <span class="italic">We are building a trusted ecosystem of people, standards, tooling and best practices for Green Software</span>

<img  src="/images/gsf.avif" alt="Description de l'image"  style="display: block; margin: auto;"/>

<!-- Allez découvrir la Green Software Foundation les principes, les outils... -->

---
layout: iframe-right
url: https://sustainability-ldscp.zatsit.fr
---

# <span style="color:#ff9900">Des outils existent pour mesurer</span>

- 🔍 Chez **zatsit** on cherche, on découvre, on teste, on partage

- 🚀 Nous avons lancé le Sustainability landscape : https://sustainability-ldscp.zatsit.fr
<br>
 
<img  src="/images/landscape-qrcode.png" alt="Description de l'image" width="200" height="200" style="display: block; margin: auto;"/>

---
layout: image
image: /images/github-green-software-directory-1.png
---
<!-- Quand on s'interesse à l'eco conception, il y a l'ademe, le collectif green-it... mais aussi la GSF -->
---
layout: image
image: /images/github-green-software-directory-top5.png
---

---
layout: image-left

# the image source
image: /images/techradar.webp
backgroundSize: contain
---

# <span style="color:#ff9900">Thoughtworks</span>

Vous connaissez sûrement : 
- Société de conseils technologiques  
- Fondée en 1993
- 49 bureaux dans 18 pays
- Martin Fowler
  - "Patterns of Enterprise Application Architecture"
  - "Agile Manifesto"
  - ....
- Une soixantaine de repositories OSS
- Et le fameux techradar 📡
 
---

# <span style="color:#ff9900">Opensource</span>

<div grid="~ cols-2 gap-4">
<div>

- Déjà en 2021, Thoughtworks décide d'opensourcer le projet.
- Certains d'entre nous découvre le cloud et sa puissance.
- D'autres en mesurent déjà les impacts...

```shell
➜ curl https://api.github.com/repos/cloud-carbon-footprint/cloud-carbon-footprint 
 | grep 'created'

"created_at": "2020-11-17T20:53:48Z",

```
</div>

<span style="transform-origin:unset;"><Tweet id="1381628247591546884" scale="0.65" /></span>


</div>

<!--
A une époque ou on commençait à jouer avec les nuages, ces gens faisaient déjà de la mesure.
-->

---
layout: default

---

# <span style="color:#ff9900">Quel rapport entre cette image et l'empreinte Carbone ?</span>
<br/>
<div style="display: flex; justify-content: center; align-items: center; height: 300px;">
  <img  src="/images/etsy_boucles.webp" alt="Description de l'image" />
</div>
---
layout: image-right
image: /images/etsy-study-1.webp
backgroundSize: 100%
---

# <span style="color:#ff9900">Une étude et une migration</span>
- **Etsy**, client de Thoughtworks, a initié le <span style="color:#ff9900">**projet lors de la migration**</span> de leur datacenter onpremise sur le cloud public.
- Comment influer une démarche pour être **plus efficace** même avec un croissance du business ?
- Comment connaître sa consommation électrique ?


<!-- Différents niveaux de PUE -->
---
layout: image-right

# the image source
image: /images/energy-proportionality.webp
backgroundSize: 100%

---

# <span style="color:#ff9900">Oui le Cloud est une excellent opportunité de réduire son empreinte</span>

- Les serveurs sont installés en prévoyance des pics de charge.
- Les serveurs sont aussi là quand il n'y a pas de charge.

---
layout: default

---
# <span style="color:#ff9900;text-align:center">Comment Thougthworks imagine la conscience et l'efficacité ?</span>

<img  src="/images/thoughtworks-green-How.webp" width="700" height="500" alt="Schema sur l'efficacité et la conscience dans le green sfotware" />


---
layout: image

# the image source
image: /images/ccf-background.webp

backgroundSize: contain
---

---
layout: default
---

# <span style="color:#ff9900">Contenu du projet ?</span>
4 repositories

![](/images/ccf-github.avif)

---
layout: image-left
image: /images/ccf-bigpicture.avif
backgroundSize: contain
---

# <span style="color:#ff9900">"Une base de départ"</span>

Un premier portail 

- Facile à installer
- Facile à connecter
- Facile à lire

- Donne envie d'aller plus loin !




---
layout: image-right

# the image source
image: /images/spared-no-expense-jurassic-park.gif
backgroundSize: 100%

---

# <span style="color:#ff9900">Des données de facturation</span>

> *"J'ai dépensé sans compter"*

Les free tiers, les réductions, la facilité et l'absence de maîtrise ont créé pas mal de surprises certaines entreprises.

> Et au deuxième jour, le DSI dit "qu'on m'embauche un FinOps !"

On fait toujours attention aux euros 💶 qui défilent, pas aux watts ⚡ qui s'échappent !


---
layout: default

---

# <span style="color:#ff9900">Exemple pour AWS</span>
<img src="/images/ccf-aws.avif" alt="schema global d'utilistation de CCF avec AWS"/>

<!-- Image AWS par Thomas Aribart -->
---
layout: iframe
url : http://localhost:3000/

---

---
layout: default

---

# <span style="color:#ff9900">Getting started</span>

```shell
npx @cloud-carbon-footprint/create-app
```

Ou

```shell
git clone --branch latest https://github.com/cloud-carbon-footprint/cloud-carbon-footprint.git
cd cloud-carbon-footprint
yarn install
yarn start
```

Les données sont mises en <span style="color:#ff9900">cache local</span>, 

mais vous pouvez utiliser une base MongoDB aussi.


---
layout: default

---

## <span style="color:#ff9900">Configuration minimaliste Pour Google Cloud Platform</span>

```sh {all|1|2|3|4|5|6|7|8|9|10|11|all} twoslash
GCP_USE_BILLING_DATA=true # less accurate as we use an average constan
# For example in us-central1, the grid emissions factor is 494 gCO2eq/kWh with CFE% of 93% (in grid and locally)
GCP_USE_CARBON_FREE_ENERGY_PERCENTAGE=true
GOOGLE_APPLICATION_CREDENTIALS=MY_SERVICE_ACCOUNT_FILE.json
GCP_BIG_QUERY_TABLE=zatsit-eco-training.all_billing_data.gcp_billing_export_resource_v1MY_TABLE
GCP_BILLING_PROJECT_ID=zatsit-eco-training
GCP_BILLING_PROJECT_NAME=zatsit-eco-training
GCP_VCPUS_PER_GKE_CLUSTER=10
GCP_VCPUS_PER_CLOUD_COMPOSER_ENVIRONMENT=10
GCP_PROJECTS=[{"id":"my-project-1", "name":"my-project-1"}, {"id":"my-project-2", "name":"my-project-2"}]
GCP_RESOURCE_TAG_NAMES=[]


ELECTRICITY_MAPS_TOKEN=MY_TOKEN
```

<arrow v-click="[12]" x1="350" y1="310" x2="195" y2="334" color="#953" width="2" arrowSize="1" />

Vous aurez préalablement : 
- <span style="color:#ff9900">**Exporter**</span> vos données de facturation dans <span style="color:#ff9900">**BigQuery**</span>
- Créer un <span style="color:#ff9900">**rôle**</span> de lecture et récupérer un <span style="color:#ff9900">**service account**</span>
- Lister les <span style="color:#ff9900">**projets**</span> que vous voulez mesurer

<!-- Le CFE n'est pas forcément bon en terme de granularité, mais globalement c'est in fine plus précis -->
---
layout: default

---

# <span style="color:#ff9900">Comment c'est calculé ?</span>

- Utiliser Electricity Map
- L'empreinte du serveur, celui du courant, l'empreinte du mec qui gère le serveur...

<span style="color:#ff9900">Formule</span>
$$ 
\begin{aligned}
Total CO2e   &= operational Emissions + embodied Emissions \\
\end{aligned}
$$

<span style="color:#ff9900">Where</span>
$$ 
\begin{aligned}
Operational emissions = (\text{Cloud provider service usage}) \\ \times (\text{Cloud energy conversion factors [kWh]}) \times (\text{Cloud provider PUE}) \\ \times (\text{grid emissions factors [metric tons CO2e]})
\end{aligned}
$$ 

<span style="color:#ff9900">And:</span>

Embodied Emissions = estimated metric tons CO2e emissions from the manufacturing of datacenter servers, for compute usage
 

<!-- PUE Énergie totale consommée par le datacenter : Cela inclut l'énergie utilisée par les serveurs, mais aussi par les systèmes de refroidissement, l'éclairage, les onduleurs (UPS), et tout autre équipement non informatique nécessaire au fonctionnement du datacenter.

Énergie consommée par les équipements informatiques : C'est uniquement l'énergie utilisée par les serveurs, le stockage, et les équipements réseau qui effectuent le travail informatique. -->
---
layout: image
image : /images/thoughtworks-estimations.avif
backgroundSize: contain
---


---
layout: image
image : /images/PUE-GCP.png
backgroundSize: contain
---

<!-- En gros faut s'approcher de 1 , tout le monde fait des efforts -->
---
layout: two-cols-header
---

# <span style="color:#ff9900">Une méthode parfaite ?</span>

::left::

### Un bon premier indicateur

- Possibilité d'utiliser <span style="color:#ff9900">Electricity Maps</span>
- Avoir une <span style="color:#ff9900">première base</span> à recroiser, à enrichir, à améliorer
- Avoir des données <span style="color:#ff9900">"indépendantes"</span> et <span style="color:#ff9900">"opensource"</span>

::right::

### Des constantes à mettre à jour

```js
export const GCP_CLOUD_CONSTANTS: CloudConstantsByProvider = {
  SSDCOEFFICIENT: 1.2, // watt hours / terabyte hour
  HDDCOEFFICIENT: 0.65, // watt hours / terabyte hour
  MIN_WATTS_MEDIAN: 0.68,
  MIN_WATTS_BY_COMPUTE_PROCESSOR: {
    // CPUs
    [COMPUTE_PROCESSOR_TYPES.CASCADE_LAKE]: 0.64,
    [COMPUTE_PROCESSOR_TYPES.SKYLAKE]: 0.65,
    [COMPUTE_PROCESSOR_TYPES.BROADWELL]: 0.71,
    [COMPUTE_PROCESSOR_TYPES.HASWELL]: 1,
    [COMPUTE_PROCESSOR_TYPES.COFFEE_LAKE]: 1.14,
    [COMPUTE_PROCESSOR_TYPES.SANDY_BRIDGE]: 2.17,
    [COMPUTE_PROCESSOR_TYPES.IVY_BRIDGE]: 3.04,
    [COMPUTE_PROCESSOR_TYPES.AMD_EPYC_1ST_GEN]: 0.82,
    [COMPUTE_PROCESSOR_TYPES.AMD_EPYC_2ND_GEN]: 0.47,
    [COMPUTE_PROCESSOR_TYPES.AMD_EPYC_3RD_GEN]: 0.45,
    // GPUs
    [COMPUTE_PROCESSOR_TYPES.NVIDIA_K520]: 26,
    [COMPUTE_PROCESSOR_TYPES.NVIDIA_A10G]: 18,
    [COMPUTE_PROCESSOR_TYPES.NVIDIA_T4]: 8,
    [COMPUTE_PROCESSOR_TYPES.NVIDIA_TESLA_M60]: 35,
    [COMPUTE_PROCESSOR_TYPES.NVIDIA_TESLA_K80]: 35,
    [COMPUTE_PROCESSOR_TYPES.NVIDIA_TESLA_V100]: 35,
    [COMPUTE_PROCESSOR_TYPES.NVIDIA_TESLA_A100]: 46,
    [COMPUTE_PROCESSOR_TYPES.NVIDIA_TESLA_P4]: 9,
    [COMPUTE_PROCESSOR_TYPES.NVIDIA_TESLA_P100]: 36,
    [COMPUTE_PROCESSOR_TYPES.AMD_RADEON_PRO_V520]: 26,
  },
```

---
layout: image
image: /images/electricitymap.avif
backgroundSize: contain
---

---
layout: default
---

# <span style="color:#ff9900">Les cloud providers vous le proposent aussi</span>

<img  src="/images/google-carbon-footprint.webp" alt="Description de l'image" />


---
layout: default

---

# <span style="color:#ff9900">Chez Amazon Web Services</span>
<img  src="/images/aws-carbon-footprint.webp" alt="Description de l'image" />

---
layout: image-right
image: /images/gsf-measure.png
backgroundSize: contain
---

# <span style="color:#ff9900">Takeways </span>

- Induire une <span style="color:#ff9900">réfléxion GreenOPS</span> : vous avez sûrement déjà un pilotage FinOps ;-)


- <span style="color:#ff9900">Sensibilisez</span> et <span style="color:#ff9900">formez-vous</span>


- Installer <span style="color:#ff9900">Cloud Carbon Footprint</span>

<!-- On peut aussi faire le choix -->

---
layout: image-left
image: /images/language-energy.avif
backgroundSize: contain
---

# <span style="color:#ff9900">Economisez les ressources</span >

1) Ai-je <span style="color:#ff9900">vraiment besoin</span> de ça ? 
2) C'est pas un peu gros comme payload ?
3) Je <span style="color:#ff9900">baisse</span>, j'<span style="color:#ff9900">éteins</span>, je <span style="color:#ff9900">décale</span>... au bon moment, au bon endroit
4) Et si j'explorai d'<span style="color:#ff9900">autres technos</span> ?


---
layout: default
---

# <span style="color:#ff9900">Green by design ?</span>

<img src="/images/gsf-design.png">

<br>

## On commence <span style="color:#ff9900">quand</span> ?

<!-- Monitorer votre equivalence CO2 votre SCI 

Software Carbon Intensity 

SCI = (E * I) + M per R -->

---
layout: image-right
image: /images/qrcode-feedback.png
---

# <span style="color:#ff9900">Merci !</span>

> "Celui qui déplace une montagne commence par déplacer de petites pierres."


 👕 Si vous avez des <span style="color:#ff9900">questions</span>, cherchez un sweat bleu dans les allées !

 📱Je reste <span style="color:#ff9900">disponible</span> sur les réseaux et dans la vraie vie !