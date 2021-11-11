<?php  
	class Hasil 
	{
		public $Nilai;
		
		function __construct($Nilai)
		{
			$this->Nilai=$Nilai;
			echo "<h1>Hasil Nilai Mahasiswa Teknik informatika</h1>";
			echo "Nilai  = $Nilai <br>";
		}

		public function Total(){
			$Total=$this->Nilai+350;
			echo "<br/><b>Nilai ditambah 6 pelajaran = $Total </b><br/>";
		}
		

		function __destruct(){
			echo "<br>nilai >400 = lulus";
            echo "<br>nilai <400 = tidak lulus";
		}
	}

	$Hasil=New Hasil(80);
	$Hasil->Total();
	
?> 
