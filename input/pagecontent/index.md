<p style="padding: 5px; border-radius: 5px; border: 2px solid maroon; background: #ffffe6; width: 65%">
<b>Brief description of this Implementation Guide</b><br>
[Add a brief description of this IG in English]
</p>

{% if site.data.info.releaselabel == 'ci-build' %}
<div style="width: 65%">
    <blockquote class="stu-note">
    <p>This Implementation Guide is not the current version. It is the continuous integration version, subject to frequent changes and intended only to follow ongoing work. The current version will be available via the canonical URL after the first release: http://interop.esante.gouv.fr/ig/fhir/[code - ig]</p>
    </blockquote>
</div>
{% endif %}


{% if site.data.info.releaselabel == 'public-comment' %}
<div style="width: 65%">
<blockquote class="stu-note">
<p>
  <b>Warning!</b>
  <br>
 This Implementation Guide is currently open for public comment. The current version is available at: http://interop.esante.gouv.fr/ig/fhir/[code - ig]
</p>
</blockquote>
</div>
{% endif %}


<!--  Uncomment if CI-SIS
<div class="figure">
    <img src="ci-sis-logo.png" alt="CI-SIS" title="CI-SIS logo" style="width:100%;">
</div>
-->

### Introduction

Define here what the IG is about (in non-expert terms, understandable by a patient). Also add the technical details on the context and the need for this IG.

The main sections of the IG are:

* The context of the IG, and the problem it solves
* What implementers must put in place
* A "Conformance resources" tab to ensure a consistent global scheme across all IGs

### Project scope

Define in a few lines the scope of the project.

Always keep the "Conformance resources" tab to ensure overall consistency across all IGs.

### Dependencies

{% lang-fragment dependency-table.xhtml %}

### Intellectual property

{% lang-fragment ip-statements.xhtml %}
