```
Route::controller(ClaintController::class)->group(function(){

    Route::get('/frontend/categoryPage/{id}/{slug}', 'CategoryPage')->name('frontend.categoryPage');

    Route::get('/frontend/subcategoryPage/{id}/{slug}', 'SubcategoryPage')->name('frontend.subcategoryPage');

    Route::get('/frontend/singlePage/{id}/{slug}', 'SinglePage')->name('frontend.singlePage');

});
```