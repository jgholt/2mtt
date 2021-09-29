
== Red Hat Solution Architect - Emergency Ansible Worshop Deployment

During normal operation, Red Hat Solution Architects and Partners should be able to run Ansible Workshops and Demos from RHPDS.  In case of a workshop ordering failure or RHPDS outage, these instructions are meant to be used as a workaround.  

*1.*  [.underline]#Build Your Virtual Environment to Run Ansible# +
It is reccomended that you have familiarity with creating a virtual environment and running Ansible,
and have tested this procedure before needing it.  Instructions can be found here:

Creating for the Mac: https://github.com/jgholt/2mtt/blob/main/ansible-aws-mac.adoc + 
Creating for Linux:  https://github.com/ansible/workshops/blob/devel/docs/setup.md

*2.* [.underline]#Order a Red Hat Open Environment from RHPDS#

https://rhpds.redhat.com Catlogs > Red Hat Open Environments > AWS Blank Open Environment

*3.* [.underline]#Obtain the Workshop Provisioner Playbooks# +

Setup (per workshop)  https://github.com/ansible/workshops/blob/devel/provisioner/README.md +
Clone the Ansible Git Repo: 
```
git clone https://github.com/ansible/workshops
```
* One suggestion would be to pre-create your extra vars files for any of the workshops you will be doing and saving them in an accessible location. 


*4.* [.underline]#Run the ansible playbook command for the desired workshop# +

```
ansible-playbook provision_lab.yml -e @extra_vars.yml

```
*4.* [.underline]#Video Walkthrough#

<p align="center">
<iframe id="kaltura_player" src="https://cdnapisec.kaltura.com/p/2300461/sp/230046100/embedIframeJs/uiconf_id/42569541/partner_id/2300461?iframeembed=true&playerId=kaltura_player&entry_id=1_ldv9j9pu&flashvars[streamerType]=auto&amp;flashvars[localizationCode]=en&amp;flashvars[leadWithHTML5]=true&amp;flashvars[sideBarContainer.plugin]=true&amp;flashvars[sideBarContainer.position]=left&amp;flashvars[sideBarContainer.clickToClose]=true&amp;flashvars[chapters.plugin]=true&amp;flashvars[chapters.layout]=vertical&amp;flashvars[chapters.thumbnailRotator]=false&amp;flashvars[streamSelector.plugin]=true&amp;flashvars[EmbedPlayer.SpinnerTarget]=videoHolder&amp;flashvars[dualScreen.plugin]=true&amp;flashvars[hotspots.plugin]=1&amp;flashvars[Kaltura.addCrossoriginToIframe]=true&amp;&wid=1_ocjok8ra" width="768" height="432" allowfullscreen webkitallowfullscreen mozAllowFullScreen allow="autoplay *; fullscreen *; encrypted-media *" sandbox="allow-forms allow-same-origin allow-scripts allow-top-navigation allow-pointer-lock allow-popups allow-modals allow-orientation-lock allow-popups-to-escape-sandbox allow-presentation allow-top-navigation-by-user-activation" frameborder="0" title="Kaltura Player"></iframe>
</p>
