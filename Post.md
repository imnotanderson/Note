#跨域

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
