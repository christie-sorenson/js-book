# First Chapter

GitBook allows you to organize your book into chapters, each chapter is stored in a separate file like this one.

TEST1234567

{% exercise %}
Define a variable `x` equal to 10.
{% initial %}
var x =
{% solution %}
var x = 10;
{% validation %}
assert(x == 10);
{% context %}
// This is context code available everywhere
// The user will be able to call magicFunc in his code
function magicFunc() {
return 3;
}
{% endexercise %}
