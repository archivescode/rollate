	$(function(){
		var itemsToShow = parseInt(12);
		console.log(itemsToShow);
		var items = {};
		for(var i=0; i < 36; i++){
			items[i] = 'ITEM ' + (i+1);
		}
  		$('#canvas').rouletteWheel({
    			items : items,
   			spinTimeTotal: 10000,
    			selected : function(key, value){
      				alert('SELECTED : ' + key + ' => ' + value);
    			},
    			spinText : 'Click Me',
    			//item index yang keluar sebagai hadiah
    			mustSelected:1,
  		});
	});

mustSelected silakan diisi dengan index item yang ingin di keluarkan sebagai hadiah

untuk prosentase keluarnya sebagai hadiah bisa dilakukan pada script php nya"Rollate for cardcell" 
