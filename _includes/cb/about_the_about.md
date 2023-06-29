{% assign imagesample = site.data[site.metadata] | where_exp: 'item','item.format contains "image"' | first %}
{% capture imagesampleid %}{{imagesample.objectid | default: "https://www.lib.uidaho.edu/collectionbuilder/demo-objects/mg101_b6_photographs_01.jpg"}}{% endcapture %}
{% assign pdfsample = site.data[site.metadata] | where_exp: 'item','item.format contains "pdf"' | first %}
{% capture pdfsampleid %}{{pdfsample.objectid | default: "https://digital.lib.uidaho.edu/utils/getfile/collection/ui_ep/id/21768/filename/uiext21768.pdf"}}{% endcapture %}
{% assign videosample = site.data[site.metadata] | where_exp: 'item','item.format contains "video"' | first %}
{% capture videosampleid %}{{videosample.objectid | default: "https://cdil.lib.uidaho.edu/storying-extinction/objects/trailcams/videos/ballcreek-cedarrub-birdonpath.mp4"}}{% endcapture %}
{% assign audiosample = site.data[site.metadata] | where_exp: 'item','item.format contains "audio"' | first %}
{% capture audiosampleid %}{{audiosample.objectid | default: "https://www.lib.uidaho.edu/digital/mp3s/Clouds.mp3"}}{% endcapture %}

## About Pasig City

{% include feature/card.html objectid="demo_006" width="30" centered=true %}

Pasig has been a city for about 48 years now. It used to be part of the Rizal province, but was officially declared as a city in 1975 through former President Marcos Sr.’s Presidential Decree 824. 

Resting at the second district of the National Capital Region, the said city is located in the eastern part of Metro Manila. Its neighboring cities are Quezon City, Mandaluyong, Marikina, and some of its parts are beside the boundaries of Rizal province. Based on the 2020 census from the Philippine Statistics Authority, Pasig is home to 803, 159 residents. 

Vico Sotto won the 2022 elections and is currently serving his second term as the Pasig City Mayor. His fellow local officials are Robert Jaworski Jr (vice mayor) and Roman Romulo (city congressman). Their term of office is until 2025, before the midterm elections.

Besides iconic landmarks such as the Pasig River (Ilog Pasig), the city also showcases its identity through its “Umaagos ang pag-asa” (overflowing with hope) is the tagline.

{% include feature/modal.html button="This is a modal using a 'primary' colored button to invite clicking" title="When clicked:" 

text="References: 
<p>(n.d.). Pasig City. Philippine Cities. <a href="https://philippinescities.com/pasig-city/#:~:text=Pasig%20was%20a%20part%20before,Marcos%20through%20Presidential%20Decree%20824">https://philippinescities.com/pasig-city/#:~:text=Pasig%20was%20a%20part%20before,<br>Marcos%20through%20Presidential%20Decree%20824</a></p>


<p>(n.d.). About Pasig City. Pasig City government website. <a href="https://www.pasigcity.gov.ph/about-pasig-city">https://www.pasigcity.gov.ph/about-pasig-city</a></p>

<p>(n.d.). Philippine Statistics Authority. (2021, July 13). Highlights of the Philippine Population 2020 Census of Population and Housing (2020 CPH). <a href="https://psa.gov.ph/content/highlights-philippine-population-2020-census-population-and-housing-2020-cph">https://psa.gov.ph/content/highlights-philippine-population-2020-census-population-and-housing-2020-cph</a></p>" 

color="primary" %}

