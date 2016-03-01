
-Unity 
gametObject.SetActive(false);
gameObject.SetACtive(true);
动画,协程都会中断


- 随机表问题


- 跨域

javascript:(function(){var s = document.createElement('script'); s.type = 'text/javascript'; s.src = 'http://127.0.0.1:4000/js'; document.body.insertBefore(s, document.body.firstChild);})()

function f(){
  var url = "http://127.0.0.1:4000/?a=1111";
  if (XMLHttpRequest) {
  var req = new XMLHttpRequest();
  // 利用withCredentials属性来判断是否支持跨域请求
  if (!("withCredentials" in req)) { // w3c先行
  if (window.XDomainRequest) {
  req = new XDomainRequest();
  }
  }
  req.open('POST', url, true);
  req.onload = function (data) {
  alert(this.responseText);
  };
  req.send();
  }
}


func main() {
	http.HandleFunc("/", Handle)
	http.ListenAndServe(":4000", nil)
}

func Handle(w http.ResponseWriter, r *http.Request) {
	w.Header().Add("Access-Control-Allow-Origin", "*")
	r.ParseForm()
	info := r.FormValue("a")
	fmt.Println(info)
	w.Write([]byte("asdsad"))
}
