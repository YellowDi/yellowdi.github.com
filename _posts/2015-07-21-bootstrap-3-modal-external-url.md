---
layout: post
title: 在 Bootstrap Modal 里使用 iframe 打开相应的链接
---
我在实际生产过程中出现的一个需求，如何在 Bootstrap 3 提供的 Modal 模拟窗里使用 iframe 打开相应的链接。

原理其实很简单，直接看代码吧。

HTML:

``` 
<a class="btn btn-primary btn-lg external" data-toggle="modal" href="http://r2vg.com" data-target="#myModal">按钮</a>
 
<!-- Modal -->
<div class="modal fade" id="myModal" tabindex="-1" role="dialog" aria-labelledby="myModalLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-body">
      </div>
      </div><!-- /.modal-content -->
  </div><!-- /.modal-dialog -->
</div><!-- /.modal -->
```

Javascript

``` 
$('a.external').on('click', function(e) {
        e.preventDefault();
        var url = $(this).attr('href');
        $(".modal-body").html('<iframe width="100%" height="100%" frameborder="0" scrolling="yes" allowtransparency="true" src="'+url+'"></iframe>');
 
    });
 
    $('#myModal').on('show.bs.modal', function () {
 
        $(this).find('.modal-dialog').css({
                  width:'40%x', //choose your width
                  height:'100%', 
                  'padding':'0'
           });
         $(this).find('.modal-content').css({
                  height:'100%', 
                  'border-radius':'0',
                  'padding':'0'
           });
         $(this).find('.modal-body').css({
                  width:'auto',
                  height:'100%', 
                  'padding':'0'
           });
    })
```

