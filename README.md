# bootstarp-switch

bootstrap-switch的下载地址：https://github.com/nostalgiaz/bootstrap-switch

bootstrap－switch的显示ON
     $("[name='my-checkbox']").bootstrapSwitch('state',true);
bootstrap－switch的显示OFF
     $("[name='my-checkbox']").bootstrapSwitch('state',false);

switch点击事件：
$('input[name="my-checkbox"]').on('switchChange.bootstrapSwitch', function(event, state) {

            if(confirm("确定要改变吗？")){
                alert("111");
            }else{
                $('[name="my-checkbox"]').bootstrapSwitch('toggleState', true);
            }
        });

$('[name="my-checkbox"]').bootstrapSwitch('toggleState', true);
这是点击 switch按钮，弹出确认框，如果点击取消的时候可以使按钮恢复到之前的状态
