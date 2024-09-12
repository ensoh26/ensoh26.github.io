<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Saint Lawrence School | City of San Diego</title>
	<link rel="icon" href="C:\Users\Paula\OneDrive\Desktop\Untitled_design-removebg-preview.png"; type="image/png">
    <style>
        body {
            font-family: century gothic;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #d6001e;
            color: white;
            display: flex;
            align-items: center;
            justify-content: space-between;
			align-items: center;
		}
        header img {
            height: 124px;
		 599px;
            margin-right: 20px;
       
        }
        nav {
            margin-left: auto;
        }
        nav ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
            display: flex;
        }
        nav ul li {
            position: relative;
        }
        nav a {
            color: white;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
            display: block;
            padding: 10px 15px;
        }
        nav ul li:hover > a {
            background-color: #078bc9;
        }
        .dropdown-content {
            display: none;
            position: absolute;
            background-color: #2653a8;
            min-width: 150px;
            z-index: 1;
            border-radius: 5px;
        }
        .dropdown-content a {
            color: white;
            padding: 10px 15px;
            text-decoration: none;
            display: block;
            text-align: left;
        }
        .dropdown-content a:hover {
            background-color: #078bc9;
        }
        nav ul li:hover .dropdown-content {
            display: block;
        }
        main {
            padding: 20px;
            background-color: #f4f4f4;
            margin: none;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            position: fixed;
            width: 100%;
            bottom: 0;
		}
        img {
            max-width: 100%;
            height: auto;
        }
        .slider {
            width: 100%;
            max-width: 10000;
			height: 500px;
            overflow: hidden;
            position: relative;
        }
        .slides {
            display: flex;
            transition: transform 0.5s ease-in-out;
        }
        .slide {
            min-width: 100%;
            
        }
        .slide img {
            width: 100%;
			height: auto; 
            display: block;
        }
        .prev, .next {
            cursor: pointer;
            position: absolute;
            top: 50%;
            width: auto;
            padding: 16px;
            margin-top: -22px;
            color: white;
            font-weight: bold;
            font-size: 18px;
            transition: 0.6s ease;
            border-radius: 0 3px 3px 0;
            user-select: none;
        }

        .next {
            right: 0;
            border-radius: 3px 0 0 3px;
        }

        .prev:hover, .next:hover {
            background-color: rgba(0, 0, 0, 0.8);
          }
		  
        #news-section {
            padding: 20px;
            text-align: center;
        }
        #news-section h1 {
            margin-bottom: 20px;
            font-size: 2em;
            color: #333;
        }
        .news-items-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
       }
        .news-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
	   }
        .news-item {
            width: 30%;
            background-color: white;
            margin-bottom: 20px;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            display: flex;
            flex-direction: column;
            text-align: left;
            transition: transform 0.3s;
        }
        .news-item:hover {
            transform: scale(1.03);
        }
        .news-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-top-left-radius: 8px;
            border-top-right-radius: 8px;
        }
        .news-item-content {
            padding: 15px;
            flex-grow: 1;
        }
        .news-item h2 {
            margin-top: 0;
            font-size: 1.5em;
        }
        .news-item p {
            margin: 5px 0 10px;
        }
        .news-item time {
            display: block;
            color: gray;
            font-size: 0.9em;
        }
        .news-item a {
            text-decoration: none;
            color: #333;
            transition: color 0.3s;
        }
        .news-item a:hover {
            color: #333;
        }
        @media screen and (max-width: 768px) {
            .news-item {
                width: 48%;
            }
        }
        @media screen and (max-width: 480px) {
            .news-item {
                width: 100%;
            }
  
		}
        #campuses-section {
            padding: 20px;
            text-align: center;
        }
        #campuses-section h1 {
            margin-bottom: 20px;
            font-size: 2em;
            color: #333;
        }
        .campuses-items-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
        }
        .campuses-item {
            width: 30%;
            background-color: white;
            margin-bottom: 20px;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            display: flex;
            flex-direction: column;
            text-align: center;
            transition: transform 0.3s;
        }
        .campuses-item:hover {
            transform: scale(1.03);
        }
        .campuses-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-top-left-radius: 8px;
            border-top-right-radius: 8px;
        }
        .campuses-item-content {
            padding: 15px;
            flex-grow: 1;
            text-align: center;
        }
        .campuses-item h2 {
            margin-top: 0;
            font-size: 1.5em;
        }
        .campuses-item p {
            margin: 5px 0 10px;
        }
        .campuses-item time {
            display: block;
            color: #653a8;
            font-size: 0.9em;
        }
        .campuses-item a {
            color: inherit;
            text-decoration: none;
        }
        .campuses-item a:hover {
            color: #4CAF50;
        }
        @media screen and (max-width: 768px) {
            .campuses-item {
                width: 48%;
            }
        }
        @media screen and (max-width: 480px) {
            .campuses-item {
                width: 100%;
            }
        }
    </style>
</head>
		
<body>

    <header>
        <img src="C:\Users\Paula\OneDrive\Desktop\Saint Lawrence School (1).png">
        
        <nav>
		<ul>
            <li>
			<a href="#Our School">Our School &#9662;</a>
			<div class="dropdown-content">
                        <a href="#X">History</a>
                        <a href="#X">Philsophy, Vision, & Mission</a>
                        <a href="#X">Goals, Objectives, & Core Values</a>
                        <a href="#X">Facilities</a>
                        <a href="#X">Acheivements</a>
                        <a href="#X">SaintLaw Hymm</a>	
                    </div>
					</li>
					<li>
            <a href="#Our Program">Our Programs &#9662;</a>
			<div class="dropdown-content">
                        <a href="#X">Admission Procedures</a>
                        <a href="#X">Curriclar Program</a>
                        <a href="#X">Extra Curriclar Program</a>
                        <a href="#X">Learning Development Assessment</a>
                        <a href="#X">Scholarships, Grants, & Discounts</a>
                    </div>
					</li>
					
					<li>
            <a href="#Our People">Our People &#9662;</a>
			<div class="dropdown-content">
                        <a href="C:\Users\Paula\OneDrive\Desktop\error.html">Administrators & Staff</a>
                        <a href="#X">Faculty</a>
                        <a href="#X">Maintencance and Transoprt</a>
                        <a href="#X">Elementary Club Officers</a>
                        <a href="#X">High School Club Officers</a>
                        <a href="#X">PTA Officers</a>
                        <a href="#X">Notable Alumni</a>
                    </div>
					</li>
					
					
            <a href="#Contact Us">Contact Us</a>
		
					
            <a href="#Enroll Now (Please)">Enroll Now (Please)</a>
			
			<ul>
        </nav>
    </header>

<div class="slider">
            <div class="slides">
                <div class="slide">
                    <img src="C:\Users\Paula\OneDrive\Pictures\20_full.jpeg">
                </div>
                <div class="slide">
                    <img src="C:\Users\Paula\OneDrive\Pictures\ac2.jpg">
                </div>
                <div class="slide">
                    <img src="C:\Users\Paula\OneDrive\Pictures\n.jpg">
				</div>
				<div class="slide">
                    <img src="C:\Users\Paula\OneDrive\Pictures\2024-05-17_212500.jpg">
				</div>
				<div class="slide">
                    <img src="https://i.imgur.com/xMDOguK.jpeg">
				</div>
            </div>
			
			 <a class="prev" onclick="changeSlide(-1)">&#10094;</a>
    <a class="next" onclick="changeSlide(1)">&#10095;</a>
        </div>
	
<main>

	<section id="news-section">
    <h1>Latest News & Updates</h1>

      <div class="news-grid">
	  
        <div class="news-item">
            <img src="C:\Users\Paula\OneDrive\Pictures\IMG20240529145625-scaled.jpg">
            <div class="news-item-content">
               <h2><a href="x">Closing Ceremonies held indoors for the FIRST TIME!</a></h2>
                <time datetime="2024-09-01">June 11, 2024</time>
                <p>The Class of 2024 had a memorable culmination of their "hard work" from months of "studying" this academic year...</p>
            </div>
        </div>
		
		<div class="news-item">
            <img src="C:\Users\Paula\OneDrive\Pictures\440941320_1234500587753104_2574745526594676928_n.jpg">
            <div class="news-item-content">
                <h2>C.A.T. and SLTC Graduation, nothing but smiles!</h2>
                <time datetime="2024-08-25">May 17, 2024</time>
                <p>It definitely wasn't easy, but these students have shown incredible "strength" and "determination" throughout. This achievement will serve as a basis for your "dedication", "perseverance", and "unwaivering commitment"...</p>
            </div>
        </div>
		
		 <div class="news-item">
            <img src="C:\Users\Paula\OneDrive\Pictures\456517146_884009686918987_526082496492161281_n.jpg">
            <div class="news-item-content">
                <h2>Into the El Filibusterismo</h2>
                <time datetime="2024-08-20">May 10, 2024</time>
                <p>Once upon a time in a far off kingdom. They wish, more than anything, more than life, more than footmen... </p>
            </div>
        </div>

   </div>
</section>

  <section id="campuses-section">
  <h1>Our Campuses</h1>
  
   <div class="campuses-items-container">

        <div class="campuses-item">
            <img src="C:\Users\Paula\OneDrive\Pictures\78_big.jpg">
            <div class="campuses-item-content">
                <h2>SAN DIEGO</h2>
                <p>1887 IBARRA STREET, CITY OF SAN DIEGO, LAGUNA</p>
            </div>
            </div>

        <div class="campuses-item">
            <img src="C:\Users\Paula\OneDrive\Pictures\ElmoreJrHigh.webp">
            <div class="news-item-content">
                <h2>ELMORE</h2>
                <p>1022 YORK STREET, ELMORE, CALIFORNIA</p>
            </div>
        </div>

        <div class="campuses-item">
            <img src="C:\Users\Paula\OneDrive\Pictures\E02-Cats-in-the-Bag.mkv_000572448.jpg">
            <div class="news-item-content">
                <h2>ALBUQUERQUE</h2>
                <p>301 LOMA COLORADO BLVD, ALBUQUERQUE, NEW MEXICO</p>
            </div>
        </div>
		
		 <div class="campuses-item">
            <img src="C:\Users\Paula\OneDrive\Desktop\xavier-school-hatley-castle.jpg">
            <div class="news-item-content">
                <h2>NORTH SALEM</h2>
                <p>1407 GRAYMALKIN LANE, NORTH SALEM, WESTCHESTER COUNTY, NEW YORK</p>
            </div>
        </div>
		
		<div class="campuses-item">
            <img src="C:\Users\Paula\OneDrive\Desktop\wb0008-8harrypotter-hogwarts50x70-933-74700.jpg">
            <div class="news-item-content">
                <h2>HIGHLANDS</h2>
                <p>1997 SOUTH HOGWARTS REIGON, HIGHLANDS, SCOTLAND</p>
            </div>
        </div>
		
		<div class="campuses-item">
            <img src="C:\Users\Paula\OneDrive\Desktop\Beigoma_Academy.png">
            <div class="news-item-content">
                <h2>BEIGOMA</h2>
                <p>2006 HIROSHI MORITA, BEIGOMA, JAPAN</p>
            </div>
        </div>
		
	</section>
   

    </main>

    <footer>
        <p>&copy; Lawrence Co. Inc.</p>
    </footer>
	
	<script>
        let index = 0;

        function showSlides(n) {
            const slides = document.querySelectorAll('.slide');
            if (n >= slides.length) {
                index = 0;
            } else if (n < 0) {
                index = slides.length - 1;
            }
            const offset = -index * 100;
            document.querySelector('.slides').style.transform = 'translateX(' + offset + '%)';
        }

        function changeSlide(n) {
            index += n;
            showSlides(index);
        }

        function autoSlide() {
            changeSlide(1);
        }

       
setInterval(autoSlide, 60000);
        showSlides(index);
    </script>

</body>
</html>
