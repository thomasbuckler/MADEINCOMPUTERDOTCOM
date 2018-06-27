--pixelpassage
--variables

x=0
score=0
size=10
pixelx=flr(rnd(123-size)+3)
pixely=-(size+100)
pixelspeed=1.5
passagex=flr(rnd(123-size)+3)

function pixelfall()
	pixely+=pixelspeed
end

function pixelpassage()
 if pixely>=(128-size) and
  passagex>=(pixelx+3) then
  pixely=130 elseif
   pixely>=(128-size) and
  passagex<=(pixelx-3) then
   pixely=130 else  
 		if pixely>=128 then
  		if passagex==pixelx then
  		pixelx=flr(rnd(123-size)+3); pixely=-(size+2); score+=1; sfx(0) elseif
  		passagex==(pixelx-1) then
  		pixelx=flr(rnd(123-size)+3); pixely=-(size+2); score+=1; sfx(0) elseif 
				passagex==(pixelx-2) then
  		pixelx=flr(rnd(123-size)+3); pixely=-(size+2); score+=1; sfx(0) elseif 
 			passagex==(pixelx+1) then
  		pixelx=flr(rnd(123-size)+3); pixely=-(size+2); score+=1; sfx(0) elseif 
				passagex==(pixelx+2) then
  		pixelx=flr(rnd(123-size)+3); pixely=-(size+2); score+=1; sfx(0)
 		end
		end
	end
end
   
function level2() 
 if score==5 and 
  pixely==-(size+2) then
 size-=1; pixelspeed+=0.3
 end
end

function level3() 
 if score==10 and 
  pixely==-(size+2) then
 size-=1; pixelspeed+=0.3
 end
end

function level4() 
 if score==15 and 
  pixely==-(size+2) then
 size-=1; pixelspeed+=0.3
 end
end

function level5() 
 if score==20 and 
  pixely==-(size+2) then
 size-=1; pixelspeed+=0.3
 end
end

function level6() 
 if score==25 and 
  pixely==-(size+2) then
 size-=1; pixelspeed+=0.3
 end
end

function level7() 
 if score==30 and 
  pixely==-(size+2) then
 size-=1; pixelspeed+=0.3
 end
end

function level8() 
 if score==35 and 
  pixely==-(size+2) then
 size-=1; pixelspeed+=0.3
 end
end

function level9() 
 if score==40 and 
  pixely==-(size+2) then
 size-=1; pixelspeed+=0.3
 end
end

function level10() 
 if score==45 and 
  pixely==-(size+2) then
 size-=1; pixelspeed+=0.3
 end
end

function movepassage()
 if btn(0) and 
 	passagex>=4 then
  passagex-=1
  if btn(4) and 
 	passagex>=7 then
  passagex-=4
  end
  elseif btn(1) and
  passagex<=(123-size) then
  passagex+=1
 	if btn(4) and
  passagex<=(120-size) then
  passagex+=4
  end
 end
-- 	if btn(2) and 
-- 		passagex>=4 then
-- 		passagex-=4
-- 		elseif btn(3) and
-- 		passagex<=(126-size) then
-- 			passagex+=4
-- 	end
end

function _update()
	pixelfall()
 pixelpassage()
 movepassage()
 level2()
 level3()
 level4()
 level5()
 level6()
 level7()
 level8()
 level9()
 level10()
end

function _draw()
--background
rectfill (1,1,126,126,0)
--border
rect (0,0,127,127,7)
--entrance
rect (pixelx-2,0,(pixelx+size+2),0,0)
--passage
rect (passagex-2,(127),(passagex+size+2),127,0)
--pixel
rectfill (pixelx,pixely,pixelx+size,(pixely+size),7)
--printing
print(score,2,2,7)
--print(passagex,50,70,7)
print(pixely,50,90,7)
if pixely>=130 then
print('game over',46,64,7)
end
if score==0 and
pixely<=10 then
print('level 001',46,56,7)
print('hold 0 to\nmove fast',46,66,7)
end
if score==5 and
pixely<=50 then
print('level 002',46,66,7)
end
if score==10 and
pixely<=50 then
print('level 003',46,66,7)
end 
if score==15 and
pixely<=50 then
print('level 004',46,66,7)
end
if score==20 and
pixely<=50 then
print('level 005',46,66,7)
end
if score==25 and
pixely<=50 then
print('level 006',46,66,7)
end
if score==30 and
pixely<=50 then
print('level 007',46,66,7)
end
if score==35 and
pixely<=50 then
print('level 008',46,66,7)
end
if score==40 and
pixely<=50 then
print('level 009',46,66,7)
end
if score==45 and
pixely<=50 then
print('level 010',46,66,7)
end

--	if btnp(0) then
--		print('true',50,80,7)
--	else
--	 print('false',50,80,7)
--	end
end