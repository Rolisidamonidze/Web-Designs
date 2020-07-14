//scroll button
var mybutton = document.getElementById("scrollBtn");
window.onscroll = function () {
  scrollFunction();
};
function scrollFunction() {
  if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
    mybutton.style.display = "block";
  } else {
    mybutton.style.display = "none";
  }
}
function topFunction() {
  document.body.scrollTop = 0;
  document.documentElement.scrollTop = 0;
}
//scroll button end

//search filter
$("#filter").keyup(function () {
  var filter = $(this).val(),
    count = 0;
  $("#results>div").each(function () {
    if ($(this).text().search(new RegExp(filter, "i")) < 0) {
      $(this).hide();
    } else {
      $(this).show();
      count++;
    }
  });
});
//search filter end

//jump to search 
$("#search_button").click(function() {
  $("#filter").focus();
  });
//jump to search end

//dynamic options
var myOptions = {
  val1 : 'All Categories',
  val2 : 'New',
  val3 : 'Used'
};
var mySelect = $('#myCategories');
$.each(myOptions, function(val, text) {
  mySelect.append(
      $('<option></option>').val(val).html(text)
  );
});