---
layout: default
---
{% if site.lang == "en-US" %}
{% capture localized_content %}{% include_relative en-us.md %}{% endcapture %}
{% else %}
{% capture localized_content %}{% include_relative pt-br.md %}{% endcapture %}
{% endif %}

{{ localized_content | markdownify }}
