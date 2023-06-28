{% assign imagesample = site.data[site.metadata] | where_exp: 'item','item.format contains "image"' | first %}
{% capture imagesampleid %}{{imagesample.objectid | default: "https://www.lib.uidaho.edu/collectionbuilder/demo-objects/mg101_b6_photographs_01.jpg"}}{% endcapture %}
{% assign pdfsample = site.data[site.metadata] | where_exp: 'item','item.format contains "pdf"' | first %}
{% capture pdfsampleid %}{{pdfsample.objectid | default: "https://digital.lib.uidaho.edu/utils/getfile/collection/ui_ep/id/21768/filename/uiext21768.pdf"}}{% endcapture %}
{% assign videosample = site.data[site.metadata] | where_exp: 'item','item.format contains "video"' | first %}
{% capture videosampleid %}{{videosample.objectid | default: "https://cdil.lib.uidaho.edu/storying-extinction/objects/trailcams/videos/ballcreek-cedarrub-birdonpath.mp4"}}{% endcapture %}
{% assign audiosample = site.data[site.metadata] | where_exp: 'item','item.format contains "audio"' | first %}
{% capture audiosampleid %}{{audiosample.objectid | default: "https://www.lib.uidaho.edu/digital/mp3s/Clouds.mp3"}}{% endcapture %}

## About Pasig City

{% include feature/card.html header="Logo of Pasig City" objectid="demo_006" width="35" centered=true %}

Pasig has been a city for about 48 years now. It used to be part of the Rizal province, but was officially declared as a city in 1975 through former President Marcos Sr.’s Presidential Decree 824. 

Resting at the second district of the National Capital Region, the said city is located in the eastern part of Metro Manila. Its neighboring cities are Quezon City, Mandaluyong, Marikina, and some of its parts are beside the boundaries of Rizal province. Based on the 2020 census from the Philippine Statistics Authority, Pasig is home to 803, 159 residents. 

Vico Sotto won the 2022 elections and is currently serving his second term as the Pasig City Mayor. His fellow local officials are Robert Jaworski Jr (vice mayor) and Roman Romulo (city congressman). Their term of office is until 2025, before the midterm elections.

Besides iconic landmarks such as the Pasig River (Ilog Pasig), the city also showcases its identity through its “Umaagos ang pag-asa” (overflowing with hope) is the tagline.

{% include feature/modal.html button="References" title="When clicked:" text="(n.d.). Pasig City. Philippine Cities. https://philippinescities.com/pasig-city/#:~:text=Pasig%20was%20a%20part%20before,Marcos%20through%20Presidential%20Decree%20824.
(n.d.). About Pasig City. Pasig City government website. https://www.pasigcity.gov.ph/about-pasig-city.   
Philippine Statistics Authority. (2021, July 13). Highlights of the Philippine Population 2020 Census of Population and Housing (2020 CPH). https://psa.gov.ph/content/highlights-philippine-population-2020-census-population-and-housing-2020-cph" color="primary"  %} 

### Include Collection Items

The template provides includes to pull your collection objects and metadata into your interpretive page, allowing you to write with your materials directly embedded in the content.

#### Include an Image

- Image --> `{% raw %}{% include feature/image.html objectid="demo_001" width="75" %}{% endraw %}`

{% include feature/image.html objectid=imagesampleid width="75" %}

#### Include a PDF

- PDF -- > `{% raw %}{% include feature/pdf.html objectid="demo_002"  width="50" %}{% endraw %}`

{% include feature/pdf.html objectid=pdfsampleid width="50" %}

#### Include a Video

- Video: `{% raw %}{% include feature/video.html objectid="demo_004" %}{% endraw %}`

{% include feature/video.html objectid=videosampleid width="75" %}

#### Include an Audio File

- Audio: `{% raw %}{% include feature/audio.html objectid="demo_003" %}{% endraw %}`

{% include feature/audio.html objectid=audiosampleid  %}

### Include Bootstrap Features

The template also provides includes to make it easier to add [Bootstrap](https://getbootstrap.com/) components to your Markdown writing.
These features allow you to better organize and highlight your content.

#### Include a Card

- Card -- > `{% raw %}{% include feature/card.html header="This is a Card" text="The card features an image from the collection as a cap" objectid="demo004" width="25" centered=true %}{% endraw %}`

{% include feature/card.html header="This is a Card" text="The card features an image from the collection as a cap" objectid="demo_001" width="25" centered=true %}

#### Include a Button 

- Buttons -- > `{% raw %}{% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" %}{% endraw %}`

{% include feature/button.html text="Button Link to Somewhere" link="https://collectionbuilder.github.io/" color="success" centered=true %}
  
#### Include an Alert

- Alerts -- > `{% raw %}{% include feature/alert.html text="this is an *alert* that 'warns' a user" color="warning" align="center" %}{% endraw %}`

{% include feature/alert.html text="This is an *alert* that 'warns' a user with centrally aligned text." color="warning" align="center"  %}

#### Include a Modal

- Modals -- > `{% raw %}{% include feature/modal.html button="This is a modal using a 'primary' colored button to invite clicking" title="when clicked:" text="A Modal will pop out a box with some more information" color="primary"  %}{% endraw %}`

{% include feature/modal.html button="This is a modal using a 'primary' colored button to invite clicking" title="When clicked:" text="A Modal will pop out a box with some more information" color="primary"  %} 
