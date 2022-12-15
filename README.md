# nonprofitdataproject


For personal reference - useful `{{ liquid tag }}` site variables: 

https://stackoverflow.com/questions/74188444/what-site-variables-can-i-use-github-pages

https://byparker.com/blog/2014/clearing-up-confusion-around-baseurl/

For example, to list a project's name, you might write: 

```
The project is called {{ site.github.project_title }}
```

To list an organization's open source repositories, you might use the following:
 
 ```
{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }})
{% endfor %}
```


