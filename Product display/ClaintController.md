```
 public function CategoryPage($id){

        $allCategory = Category::findOrFail($id);

        $allProduct = Product::where('category_id', $id)->latest()->get();

        return view('frontend.categoryPage', compact('allCategory', 'allProduct'));

    }


    //data show Subcategory_page

    public function SubcategoryPage($id){

        $allSubcategory = Subcategory::findOrFail($id);

        $allProduct = Product::where('subcategory_id', $id)->latest()->get();

        return view('frontend.subcategoryPage', compact('allSubcategory', 'allProduct'));

    }

	public function SinglePage(){

        return view('frontend.singlePage');

    }
```