# Release Notes

## 0.1.0-dev

__Date:__ [Under Developement](https://github.com/{{ cookiecutter.github_username}}/{{ cookiecutter.github_reponame}}/issues/1)

__Features__

- ...
- initial setup of project.

__Fixes__

- ...

<!-- create links for github issues -->
<script src="https://padolsey.github.io/findAndReplaceDOMText/src/findAndReplaceDOMText.js"></script>
<script>
    var repo = '{{ cookiecutter.github_username}}/{{ cookiecutter.github_reponame}}';
    findAndReplaceDOMText(document.querySelector('[role="main"]'), {
      find: /#(\d+)/g,
      replace: function(portion, match){
        var el = document.createElement("a");
        el.setAttribute('href', 'http://github.com/'+ repo +'/issues/'+ match[1]);
        el.setAttribute('target', '_blank');
        el.innerHTML = portion.text;
        return el;
        }
    });
</script>