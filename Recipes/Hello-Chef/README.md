### Project Creation

Create the following file

*hello-chef.rb*

```ruby
file 'welcome.txt' do                 <-------  1
 content 'Hello Chef!, Welcome.'      <-------  2
end                                   <-------  3
```

1] *file* is a *resource* that can be used to manage a file on a computer. 
It accepts a string parameter specifying the path to the file, which can be specified either in single or double quotes.

The *do* keyword marks the beginning of the block.

2] *content* is an *attribute* that can be used to specify the content that has to be written to the file resource. 

It can be thought of as a parameter to the resource, 
so the string 'Hello Chef!, Welcome.' is passed as the value of the *content* attribute to the *file* resource.

3] The *end* keyword marks the end of the block.


```sh
droid@droidserver:~/onGit/Chef-Tryouts/Recipes/Hello-Chef$ which chef-apply
/usr/bin/chef-apply
droid@droidserver:~/onGit/Chef-Tryouts/Recipes/Hello-Chef$ chef-apply hello-chef.rb 
Recipe: (chef-apply cookbook)::(chef-apply recipe)
  * file[welcome.txt] action create
    - create new file welcome.txt
    - update content in file welcome.txt from none to 46c86c
    --- welcome.txt	2016-11-10 20:32:50.479729946 -0500
    +++ ./.chef-welcome20161110-17330-9mbuf3.txt	2016-11-10 20:32:50.479729946 -0500
    @@ -1 +1,2 @@
    +Hello Chef!, Welcome.
```

The generate file is

*welcome.txt*

```
Hello Chef!, Welcome.
```
