```

public function home(){
$allProduct = Product::latest()->limit(1)->offset(3)->get();
return view('frontend.home_page', compact('allProduct'));
}
```