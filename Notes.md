steps:-
    HTML:-
         1. Added js and css files in html with added google font roboto-body and sen -logo
         2. Added two `<div>` tags with Navbar and sidebar classes
                      a. Navbar- a.Navbar-container class
                                a.logo-container - added a `<h1>` with class "logo" and with content-flakes
                                b.menu-container -   1.in menu container i have added a `<ul>` with menu-list class
                                                     2. created multiple list in `<ul>` with class="menu-list-item"list with names -home ,movies ,series,popular,trends
                                c.profile-container -1.  in profile container make  a profile-picture class and and add image using `<img/>`
                                                     2. make profile-text-container `<div>` and inside that make a class=profile-text and go to font awasome a find a arrow icon and
                                                        paste under profile-text
                                                     3.make a toggle class for a darkmode and lightmode
                                                     4. make a toggle-ball class to change modes

    b. sidebar :- 1. left-menu-icons -in sidebar i needs to add some icons from font awasome  like - Home ,search , users ,bookmarks ,tv ,hourglass,shoping cart and give them left-menu-icon class

    c.Content :- 1. make a class container and inside that make another div with content-container for whole apps 's content
                                    2.content-container
                                      a.featured-content - a.added inline css becoz we wants to make it dynamic image ,added a linear-gradient color to match with below colr
                                                           b.now in this section we wants to show title ,an image , few call to action button , a small description
                                                           c. featured-title - it will be a image f-t-1.png
                                                           d. featured-desc - it will be paragraph about featured content
                                                           e.featured-button - it will cta button -WATCH

    b.movie-list-container -
                                                           a. movie-list-title - make an`<h1>` and write "NEW RELEASES"
                                                           b. movie-list-wrapper - inside this we will add slider to slide b/w diff movies
                                                              a. movie list-
                                                                        a. movie-list-item :- 1.inside this will be a movie  with its image ,button ,desc,button
                                                                                              2.movie-list-item-img - it will have a `<img/>`
                                                                                              3. movie-list-item-title- movie name will be there in a `<span>`
                                                                                              4. movie-list-item-desc   - little bit description about titled movie in form of a `<p>`
                                                                                              5. movie-list-item-button -- WATCH
                                                                          b. replicate same movie-list-item 5-7 items
                                                                b.   Arrow - ">" sign
                                      c. replicate all movie-list-container 3-4 times to make diffrent section on content-container and make changes accordingly
    d. and also add featured content after 2 section like that and make changes accordingly
                                      e. add js file

   CSS:-
        1. set default margin and padding to whole content
        2. Navbar design- a.in navbar class given 100% width and a bg color
                       a.navbar-container class design - display: flex to make logo,menu,profile in a row , align-item: center ,bgColor , p-50px,,height-100/%
                                 a.logo-container design - flex1 , added  fontFAM , font size,colr

    b. menu-container design - flex6 ,
                                                    1.menu-list -make it flex to display in horizonatal and make list-style:none
                                                              1.menu-list-item => added a margin between all menu items and make Home little but bolder than all other iitems
                                 c.profile container design - flex2, dispaly:flex ,align item:center  , justify-content:end
                                                     1.profile-picture class design- here i given w32px,h32px and border radius 50% to make profile picture small and circular , object-fit:cover to take whole cicle evenly
                                                     2. profile-text-container design-  margin 0 20px
                                                     3.toggle - 1.add width:40px,height:20px ,bgcolr ,radius50% , and go to font awasome and take two icons moon and sun to show darkmode
                                                                  and daymode and also add justify-content : space around and align-items :center ,position:relative
                                                                3.toggle-icon - give toggle icons a gold col
                                                                4. toggle-ball -w18,h18,colr:black ,positio:absolute, rign1, radius50 , cursor:pointer

    3. sidebar :- a.sidebar --in sidebar class i given 100% hieght and 50px width ,we wants to keep our sidebar fixed in whole web so added position:fixed  ,here icons will
                         be there so make it display:flex ,flex-direction:cols , padding :60px on top , justify-content:space-around, align-items :center
                      b.left-menu-icons --colr white , font size 20px , margin bottom:40px  , now icons will look great in sidebar
        4. container :- a. given min-height: calc(100vh-50px) , 50px minus of navbar, give bg color :black  , colr :white
                        b.content-container -- margin-left:50px for sidebar space,
                          a.featured-content- 1. height:50vh , added inline css becoz we wants to make it dynamic image ,added a linear-gradient color to match with below colr , padding-50px
                                              2.featured -title - it is a image so set its size first  width:200px
                                              3. featured -desc - width :500px ,color:lightgray , margin :30px 0 with titile and buttons
                                              4. featured-button -- given bg colr:green , padding :10 20px ,border-radius:10px,colr:white , border:none , outline :none , bold

    b.movie-list-container -1.p20,
                                                  2movie-list-wrapper - position:relative
                                                  2. movie-list - make all movies list as display:flex  ,h300,align-item:center
                                                  3.movie-list-item - mr30 , position :relative
                                                  4. movie-list-item-img -- w270 , h200n , object-fit:cover ,transition:all 1s ease-in-out ,
                                                  5. Animation- on hovring on movie-list-item it should show transformation by scale(1.2) ,m :0 30px  , opacity :0.5 ,transition:all 1s ease-in-out
                                                  6. movie-list-item-title -- bgcolr- ,p:0 10px ,font-size:32px ,font-weight :bold  , position:absolute ,top20% ,l50 , transition:all 1s ease-in-out
                                                  7.movie-list-item-desc --bgcolr , p10,fontsize14,p: absolute , font-size:16px,top30%, w230 to not overflow ,opacity :0 ,transition:all 1s ease-in-out
                                                  8.movie-list-item-button  --p10 , bgcolr:green , colr:whitem , radius10 ,outline:none ,cursor:pointer ,absolute ,b20,l50  ,opacity :0 ,transition:all 1s ease-in-out
                                                  9.Arrow -- font-size120 ,absolute ,t90,bgclr,right:0 ,clr:gray,cursor:pointer ,opacity
                         c. design ofother sections will be same as above
                         d. add media query to make app responsive like when screen size is more than 940 diapper menu bar

JS:--
      1. Now here i will change dyanmic things on my page to make page intractive like adding functionality to arrow ,toggle
      2.Arrow - add eventlistener "click" on arrrow , movie-list should move across x-axis so use movielist[i].style.tranform=translateX(100px) , here overflowing so make movie-list-wrapper make oveflow:hidden
      3.using computedStyleMap capture the initial style on ith movie and using get get its x value and subtract 300 px so that it can move towards left by 300px
      4.but we wants that it should not indefinite move , there should be a limit and after that it should starts from starting so for that first i have calculate  total numbr of images in movielist and by each click i will increse clickcounter  , if itemnumber -(4+clickcounter)>0 then subtract by 300px and move left otherwise trunback it in initial style and set clickcounter=0
      5.

    1. now lets design toggle
      2. access toggle ball using queryselctor(.toggle-ball)
      3. select all elementson that we wants to apply mode serivce
      4. add click eventlistener on ball such that on clicking all items.classlist.toggle("active")
      5. after clicking  make ball.classlist.toggle("active") so that it can look like whiter
      6. we can aslo add some transition  on toggle-ball transition 1s ease  all
      7.but we know this design is not responsive so to fix that i will add media query
      8. after making responsive our crousel not showing all limit items use window object
