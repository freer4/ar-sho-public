---
title: Tau Lexicon | Warhammer 40K
navtext: Lexicon
description: Warhammer 40K Tau Lexicon in a searchable database format. Reference for the Tau language. 
hero: "/assets/images/tau-water-caste-envoy.jpg"
heroalt: "Tau Empire water caste members"
---
# Tau Lexicon

{% include underconstruction.html %}

Based initially on this [Tau-English dictionary](https://commanderfarsight.deviantart.com/art/Tau-English-Dictionary-164979522), this repository will contain all canon instances of the Tau language for reference.

Check out this [Tau name generator](http://www.fantasynamegenerators.com/warhammer-40k-tau-names.php){:target="_blank"} if you're looking to add some depth to your army. 

<select id="part">
  <option value="">Part of speech</option>
  <option value="a">Adjective</option>
  <option value="v">Verb</option>
  <option value="n">Noun</option>
  <option value="p">Proper noun</option>
</select><input type="text" id="search" />

| Tau | - | Definition | Tags | References |
|:---|:---:|:---|:---|:---:|
{% for word in site.data.lexicon %}|{{word[0]}}|{{word[1]}}|{{word[2]}}|{{ word[3] | join: ', ' }}|{{ word[4] | join: ', ' }}|
{% endfor %}{: #collection}

<script type="text/javascript">var collection = {{site.data.lexicon | jsonify}};

var search = document.getElementById("search");
var table = document.getElementById("collection");
var part = document.getElementById("part");

for (var i = 0, l = collection.length; i<l; ++i){
  for (var j = 0, k = collection[i].length; j<k; ++j){
    if (typeof collection[i][j] === 'string'){
      collection[i][j] = collection[i][j].toLowerCase();    
    }
  }
}

var doSearch = function(e){
  var rows = table.querySelectorAll("tr");
  var val = search.value.toLowerCase();
  if (val.length || part.value.length){
    for(var i = 1, l = rows.length; i<l; ++i){
        rows[i].classList.add("hidden","stripe");
    }
    var s = 0;
    for(var i = 0, l = collection.length; i<l; ++i){
      if ((!val.length || collection[i][0].indexOf(val) === 0 || collection[i][2].includes(val)) && (!part.value.length || collection[i][1] === part.value)){
        rows[i+1].classList.remove("hidden");
        if (s%2){
          rows[i+1].classList.remove("stripe");  
        }
        s++;
      }
    }
  } else {
    for(var i = 1, l = rows.length; i<l; ++i){
        rows[i].classList.remove("hidden","stripe");      
    }
  }
}

search.addEventListener("input", doSearch);
part.addEventListener("input", doSearch);

</script>
