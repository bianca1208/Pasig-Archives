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

References: 
<p>(n.d.). Pasig City. Philippine Cities. <a href="https://philippinescities.com/pasig-city/#:~:text=Pasig%20was%20a%20part%20before,Marcos%20through%20Presidential%20Decree%20824">https://philippinescities.com/pasig-city/#:~:text=Pasig%20was%20a%20part%20before,<br>Marcos%20through%20Presidential%20Decree%20824</a></p>


<p>(n.d.). About Pasig City. Pasig City government website. <a href="https://www.pasigcity.gov.ph/about-pasig-city">https://www.pasigcity.gov.ph/about-pasig-city</a></p>

<p>(n.d.). Philippine Statistics Authority. (2021, July 13). Highlights of the Philippine Population 2020 Census of Population and Housing (2020 CPH). <a href="https://psa.gov.ph/content/highlights-philippine-population-2020-census-population-and-housing-2020-cph">https://psa.gov.ph/content/highlights-philippine-population-2020-census-population-and-housing-2020-cph</a></p>

 {% include feature/modal.html button="This is a modal using a 'primary' colored button to invite clicking" title="When clicked:" text="In her candidacy as vice president of the Philippines, Leni Robredo stood against male candidates who had previously held positions in the national government. In one memorable debate, she said: “I am a mother who will always look after her children. I will always look after our country. To the six of us, may the best woman win.” She was elected Vice President of the Philippines in 2016.

It was not part of her plan to make it this big in politics. Her childhood memories were those of helping her father’s destitute clients and this imbibed in her a sense of duty for people “at the seams of society.” 

Leni was propelled to the national political scene after the tragic death of her husband in a plane crash in August 2012. She was urged her to run for Congress, and she won a seat representing Camarines Sur province. And by surprise, in 2016, she was asked to be the vice presidential candidate to the Liberal government’s frontrunner Mar Roxas.

Leni won by a margin of 200,000 votes ahead of Ferdinand Marcos Jr. the son of the late dictator President Marcos. Leaving him unsatisfied with the results, Marcos filed an election protest in the Supreme Court. She soon found herself out of the cabinet formed by the current populist President Rodrigo Duterte, who favors the Marcos family. That and an onslaught of propaganda against Leni has not stopped her from going to the farthest reach of the country to help the poor build their homes and make a better life. 

Leni has spoken out against President Duterte’s brutal drug war, which saw the killings of suspected drug dealers in the slums of Manila. She is effectively the leader of the opposition although she prefers to roam the countryside for her “Angat Buhay” (Lifting Life) social campaign for the underprivileged. 

Involvement of sectors in development

Angat Buhay seeks to empower the marginalized sector, including women, in partnership with the private sector and civil society partners.

Part of this endeavor is putting an end to domestic abuse and empowering women toward financial independence. In one interview, she said "Karamihan sa nasalubong namin na mga problema, kahit inaabuso na, parang they would choose to go back to the abusive environment dahil ang pakiramdam niya, hindi niya kayang buhayin iyong sarili niya at saka mga anak." 

(Most of the problems that we’ve encountered involved women who chose to remain in an abusive environment. This is because a woman feels like she can't provide for herself and her children.)

Leni tries to address this by equipping women with skills that would help them start a business and become entrepreneurs. Leni explains that “academic studies have shown that in order to close the gender gap, at least four things should happen: first, make it safe and fair for women to do trade-related businesses; second, bring more women into the workforce and achieve gender parity in the workplace; third, make spaces for female-led enterprises; and fourth, facilitate equal access to technology.”

Leni has taken up the torch to keep the dying flames of democracy alive. The space that she creates for women empowerment sparks the flame." color="primary" %}
