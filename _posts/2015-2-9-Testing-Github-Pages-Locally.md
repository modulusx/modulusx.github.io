---
layout: post
title: Authoring Github Pages articles locally
---

### Less waiting, more writing
We don't want to spend all of our time pushing commits to github, so lets run a local instance of github-pages and get busy writing articles instead.

To simplify this, I've created [test-pages](https://github.com/modulusx/test-pages) that contains a Vagrantfile and Ansible playbook that will stand up and provision your own box. Assuming you have Vagrant and Ansible, it's as simple as:
{% highlight git %}
git clone https://github.com/modulusx/test-pages.git
cd test-pages
export GHP_REPO=https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git
vagrant up
{% endhighlight %}

Now just edit your source code in test-pages/repo until [your site](http://localhost:8000) looks good. Commit and push and you're done!
