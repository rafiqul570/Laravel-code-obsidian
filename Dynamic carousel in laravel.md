```
<div id="carouselExampleSlidesOnly" class="carousel slide" data-ride="carousel">
<div class="carousel-inner">
@foreach ($allProduct as $key => $data)
<div class="carousel-item {{$key == 0 ? 'active':''}}">
@if ($data->product_img)
<h3 class="text-center">{{$data->product_name}}</h3>
<h6 class="text-center"><span class="text-danger">Price</span> : ${{$data->product_price}}</h6>
<img class="d-block w-80" src="{{asset('uploads/image/'.$data->product_img)}}">
<a href=""><span class="text-dark">Buy now</span></a>
@endif
</div>
@endforeach
</div>
</div>
```