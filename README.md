// Game-of-fifteen-code

.model small
.code
org 100h
.386



start:

	mov ax, 0600h
	mov bh, 5Fh
	mov cx, 0000h
	mov dx, 184Fh 
	int 10h 

	;printing my name
	
	mov ah, 13h
	mov al, 00
	mov bh, 00
	mov bl, 2Fh
	lea bp, Name1  ;By Sharmin Akhter
	mov cx, 18
	mov dh, 22
	mov dl, 05
	int 10h
	
	; for writing on screen msg
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 4Fh
	lea bp, screen1  ;It will print 'press T for up'
	mov cx, 14
	mov dh, 15
	mov dl, 60
	int 10h 
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 4Fh
	lea bp, screen2  ; It will print 'press V for down'
	mov cx, 16
	mov dh, 17
	mov dl, 60
	int 10h 
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 4Fh
	lea bp, screen3  ; It will print 'press h for right'
	mov cx, 17
	mov dh, 19
	mov dl, 60
	int 10h 
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 4Fh
	lea bp, screen4  ; It will print 'press D for left'
	mov cx, 17
	mov dh, 21
	mov dl, 60
	int 10h 
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 4Fh
	lea bp, screen5  ;It wil print 'press Q for quit'
	mov cx, 17
	mov dh, 23
	mov dl, 60
	int 10h 
	
	;It will print 'Game of 15'

	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 9Fh
	lea bp, Titl   
	mov cx, 10
	mov dh, 03
	mov dl, 32 
	int 10h 
	 
	;number printing 
	
	mov ah, 13h 
	mov al, 00 
	mov bh, 00 
	mov bl, 5Fh
	lea bp, Line1
	mov cx, 02
	mov dh, 07
	mov dl, 46
	int 10h 
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line2
	mov cx, 02
	mov dh, 10
	mov dl, 46
	int 10h   
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line3
	mov cx, 02
	mov dh, 13
	mov dl, 46
	int 10h   
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line4
	mov cx, 2
	mov dh, 16
	mov dl, 46
	int 10h 
	
	mov ah, 13h 
	mov al, 00 
	mov bh, 00 
	mov bl, 5Fh
	lea bp, Line5
	mov cx, 2
	mov dh, 07
	mov dl, 39
	int 10h 
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line6
	mov cx, 2
	mov dh, 10
	mov dl, 39
	int 10h   
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line7
	mov cx, 2
	mov dh, 13
	mov dl, 39
	int 10h   
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line8
	mov cx, 2
	mov dh, 16
	mov dl, 39
	int 10h 
	
	mov ah, 13h 
	mov al, 00 
	mov bh, 00 
	mov bl, 5Fh
	lea bp, Line9
	mov cx, 2
	mov dh, 07
	mov dl, 32
	int 10h 
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line10
	mov cx, 2
	mov dh, 10
	mov dl, 32
	int 10h   
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line11
	mov cx, 2
	mov dh, 13
	mov dl, 32
	int 10h   
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line12
	mov cx, 2
	mov dh, 16
	mov dl, 32
	int 10h 
	
	mov ah, 13h 
	mov al, 00 
	mov bh, 00 
	mov bl, 5Fh
	lea bp, Line13
	mov cx, 2
	mov dh, 07
	mov dl, 25
	int 10h 
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line14
	mov cx, 2
	mov dh, 10
	mov dl, 25
	int 10h   
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line15
	mov cx, 2
	mov dh, 13
	mov dl, 25
	int 10h      
	
	
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, Line16 
	mov cx, 02
	mov dh, 16
	mov dl, 25
	int 10h 
	
	;For printing box
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box1 
	mov cx, 27
	mov dh, 05
	mov dl, 23
	int 10h 
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box2 
	mov cx, 27
	mov dh, 08
	mov dl, 23
	int 10h 
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box3
	mov cx, 27
	mov dh, 11
	mov dl, 23
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box4
	mov cx, 27
	mov dh, 14
	mov dl, 23
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box5
	mov cx, 27
	mov dh, 17
	mov dl, 23
	int 10h
	
	;drawing box for dh
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box6 
	mov cx, 03
	mov dh, 06
	mov dl, 22
	int 10h 
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box7 
	mov cx, 03
	mov dh, 07
	mov dl, 22
	int 10h 
	

   
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box8
	mov cx, 03
	mov dh, 09
	mov dl, 22
	int 10h 
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box9
	mov cx, 03
	mov dh, 10
	mov dl, 22
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box10
	mov cx, 03
	mov dh, 12
	mov dl, 22
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box11
	mov cx, 03
	mov dh, 13
	mov dl, 22
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box12
	mov cx, 03
	mov dh, 15
	mov dl, 22
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box13
	mov cx, 03
	mov dh, 16
	mov dl, 22
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, boxm
	mov cx, 03
	mov dh, 06
	mov dl, 49
	int 10h
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box14
	mov cx, 03
	mov dh, 07
	mov dl, 49
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box15
	mov cx, 03
	mov dh, 09
	mov dl, 49
	int 10h
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box16
	mov cx, 03
	mov dh, 10
	mov dl, 49
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box17
	mov cx, 03
	mov dh, 12
	mov dl, 49
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box18
	mov cx, 03
	mov dh, 13
	mov dl, 49
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box19
	mov cx, 03
	mov dh, 15
	mov dl, 49
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box20
	mov cx, 03
	mov dh, 16
	mov dl, 49
	int 10h
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box21
	mov cx, 02
	mov dh, 06
	mov dl, 28
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box22
	mov cx, 03
	mov dh, 07
	mov dl, 28
	int 10h
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box23
	mov cx, 02
	mov dh, 09
	mov dl, 28
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box24
	mov cx, 03
	mov dh, 10
	mov dl, 28
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box25
	mov cx, 03
	mov dh, 12
	mov dl, 28
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box26
	mov cx, 03
	mov dh, 13
	mov dl, 28
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box27
	mov cx, 03
	mov dh, 15
	mov dl, 28
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box28
	mov cx, 03
	mov dh, 16
	mov dl, 28
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box29
	mov cx, 03
	mov dh, 06
	mov dl, 35
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box30
	mov cx, 03
	mov dh, 07
	mov dl, 35
	int 10h
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box31
	mov cx, 03
	mov dh, 09
	mov dl, 35
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box32
	mov cx, 03
	mov dh, 10
	mov dl, 35
	int 10h
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box33
	mov cx, 03
	mov dh, 12
	mov dl, 35
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box34
	mov cx, 03
	mov dh, 13
	mov dl, 35
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box35
	mov cx, 03
	mov dh, 15
	mov dl, 35
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box36
	mov cx, 03
	mov dh, 16
	mov dl, 35
	int 10h
	
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box37
	mov cx, 03
	mov dh, 06
	mov dl, 42
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box38
	mov cx, 03
	mov dh, 07
	mov dl, 42
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box39
	mov cx, 03
	mov dh, 09
	mov dl, 42
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box40
	mov cx, 03
	mov dh, 10
	mov dl, 42
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box41
	mov cx, 03
	mov dh, 12
	mov dl, 42
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box42
	mov cx, 03
	mov dh, 13
	mov dl, 42
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box42
	mov cx, 03
	mov dh, 15
	mov dl, 42
	int 10h
	
	mov ah, 13h 
	mov al, 00
	mov bh, 00
	mov bl, 5Fh
	lea bp, box43
	mov cx, 03
	mov dh, 16
	mov dl, 42
	int 10h
	
   
   ; Set cursor position
	
	mov ah, 2
    mov dh, 16
	mov dl, 25
	mov bh, 00h
	int 10h
	
	
	
	INPUT5:
	
	mov ah, 08h 
	int 21h 
	cmp al, 't'
	je up
	cmp al,'v'
	je down
    cmp al, 'h' 
    je right  
	cmp al, 'd'
	je left
	cmp al, 'q'
	je ENDPROGRAM 
	jmp INPUT5
	
	
	UP:  
   ;cursor for upperbound
   
   cmp dh,7
   je INPUT5
   
   ; To get cursor position and size info
   
   mov ah,3
   mov bh,00
   int 10h     
   
   add dh,-3 		  ; This is the space between two numbers
   
   
   ;To relocate the cursor with current position
   
   mov ah,2
   mov dl,dl
   mov dh,dh
   mov bh,00
   int 10h  
  
   mov ah,08h
   mov bh,00
   int 10h
   mov bl, ah   
   
   add dh, 3   ;space between two numbers
   
   
   ;sets cursor
  
   mov ah, 2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h
   
   
   ;To replace uppernumber
   mov ah,09h
   mov al,al
   mov bl,bl
   mov cx,01h
   int 10h   
   
   add dh, -3  
  

  ;Moves cursor back up   
   
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h
   
   
   ;Outputs blank space
   mov ah, 09h
   mov al, 00h
   mov bh, 0
   mov cx,1
   mov bl,bl
   int 10h
   
   
   ;Get cursor position and size info
   mov ah,3
   mov bh,00
   int 10h   
   
   add dl, 1
   
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,00
   mov dl,dl
   int 10h
   
   
   ;This reads and stores number information
   mov ah,08h
   mov bh,00
   int 10h

   mov bl,ah   
  
   add dh, 3   
   
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h
 
   
   mov ah,09h
   mov al,al
   mov bl,bl
   mov cx,01h
   int 10h  

   
   mov ah,3
   mov bh,00
   int 10h

   add dh,-3   
   
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   mov ah,09h
   mov al,00h
   mov bl,79h
   mov cx,01h
   int 10h  

   ;Get cursor position and size information
   mov ah,3
   mov bh,00
   int 10h

   add dl, -1
   
   ;sets cursor to current blank space
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h
   
   jmp INPUT5
   
   DOWN:

   ;Get cursor position and size info
   mov ah,3
   mov bh,00
   int 10h
   
   ;For lowerbound
   cmp dh,16
   je INPUT5   
   
   ;when space bewteen number change
   add dh,3 
   ;moves cursor up
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,00
   mov dl,dl
   int 10h
   
   ;read above number and store
   mov ah,08h
   mov bh,00
   int 10h

   mov bl, ah
   add dh,-3  
   
   ;cursor back to blank spot again
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h
   
   ;For upper number into blank spot
   mov ah,09h
   mov al,al
   mov bl,bl
   mov cx,01h
   int 10h     
   
   add dh,3 
   
   ;cursor goes back up   
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   ;For Outputs blank space
   mov ah, 09h
   mov al, 00h
   mov bh, 0
   mov cx,1
   mov bl,bl
   int 10h

   ;ToGet cursor position and size info
   mov ah,3
   mov bh,00
   int 10h
   
   add dl, 1
   
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,00
   int 10h
   ;This reads character above and store information
   mov ah,08h
   mov bh,00
   int 10h
   
   mov bl,ah  
   ; it will change the number position when dh space change
   add dh, -3
   
   ;It will bring the cursor back to original blank spot
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   ;swap the top with blank
   mov ah,09h
   mov al,al
   mov bl,bl
   mov cx,01h
   int 10h  

   ;To Get cursor position and size info
   mov ah,3
   mov bh,00
   int 10h

   add dh,3
         
   ;It sets cursor
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   mov ah,09h
   mov al,00h
   mov bl,79h
   mov cx,01h
   int 10h  

   ;Get cursor position and size info
   mov ah,3
   mov bh,00
   int 10h

   add dl, -1
   ;sets cursor to blank space
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h
   jmp INPUT5
   
   
   LEFT: 

   ;Get cursor position and size info
   mov ah,3
   mov bh,00
   int 10h
   
   ;left side
   cmp dl,25
   je INPUT5
   add dl,-7   
   ;moves cursor to position above
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,00
   int 10h
   
   ;read amd store 
   mov ah,08h
   mov bh,00
   int 10h

   mov bl, ah  
   
   add dl,7
   ;cursor to blank
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   ;swap
   mov ah,09h
   mov al,al
   mov bl,bl
   mov cx,01h
   int 10h     
   
   add dl,-7
   
   ;cursor into new blank  
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   mov ah, 09h
   mov al, 00h
   mov bh, 0
   mov cx,1
   mov bl,bl
   int 10h

   ;Get cursor position and size info
   mov ah,3
   mov bh,00
   int 10h
  
   add dl, 1
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,00
   mov dl,dl
   int 10h

   mov ah,08h
   mov bh,00
   int 10h

   mov bl,ah   
   add dl, 7   
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h
  
   ;swap right to right with blank
   mov ah,09h
   mov al,al
   mov bl,bl
   mov cx,01h
   int 10h  

   ; To Get cursor position and size info
   mov ah,3
   mov bh,00
   int 10h

   add dl,-7        
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   ;It will create new blank space 
   mov ah,09h
   mov al,00h
   mov bl,79h
   mov cx,01h
   int 10h  

   ;Get cursor position and size info
   mov ah,3
   mov bh,00
   int 10h

   add dl, -1
   
   ;It will bring the cursor to blank 
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   jmp INPUT5

RIGHT:
   ;Get cursor position and size info
   mov bh,00
   int 10h
   
   ;right side
   
   cmp dl,46
   je INPUT5
   add dl,7  
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,00
   mov dl,dl
   int 10h
   
   mov ah,08h
   mov bh,00
   int 10h

   mov bl, ah   
   add dl,-7   
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   ;swap 
   mov ah,09h
   mov al,al
   mov bl,bl
   mov cx,01h
   int 10h     
   
   add dl,7   
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   ;Outputs blank space
   mov ah, 09h
   mov al, 00h
   mov bh, 0
   mov cx,1
   mov bl,bl
   int 10h

   ;Get cursor position and size info 
   mov ah,3
   mov bh,00
   int 10h
   
   add dl, 1
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,00
   int 10h

   mov ah,08h
   mov bh,00
   int 10h

   mov bl,ah   
   add dl, -7
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h
  
   ;swap 
   mov ah,09h
   mov al,al
   mov bl,bl
   mov cx,01h
   int 10h  

   ;cursor info for next operation
   mov ah,3
   mov bh,00
   int 10h

   add dl,7    
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   mov ah,09h
   mov al,00h
   mov bl,79h
   mov cx,01h
   int 10h  

   mov ah,3
   mov bh,00
   int 10h

   add dl, -1
   
   ;cursor to blank space for next operation
   mov ah,2
   mov dh,dh
   mov dl,dl
   mov bh,0
   int 10h

   jmp INPUT5
   
   
   ENDPROGRAM:
   MOV AX,0600H    ;06 TO SCROLL & 00 FOR FULLJ SCREEN
   MOV BH,71H    ;ATTRIBUTE 7 FOR BACKGROUND AND 1 FOR FOREGROUND
   MOV CX,0000H    ;STARTING COORDINATES
   MOV DX,184FH    ;ENDING COORDINATES
   INT 10H        ;FOR VIDEO DISPLAY
   MOV AH,4CH    ;RETURN TO DOS MODE
   INT 21H
	
	
   
   ret
             
   box1  db '--------------------------',13,10,'$'
   box2  db '--------------------------',13,10,'$'
   box3  db '--------------------------',13,10,'$'
   box4  db '--------------------------',13,10,'$'
   box5  db '--------------------------',13,10,'$'
   box6  db '|',13,10,'$'
   box7  db '|',13,10,'$' 
   box8  db '|',13,10,'$' 
   box9  db '|',13,10,'$' 
   box10 db '|',13,10,'$'
   box11 db '|',13,10,'$'
   box12 db '|',13,10,'$'
   box13 db '|',13,10,'$'
   boxm  db  '|',13,10,'$'
   box14 db '|',13,10,'$'
   box15 db '|',13,10,'$'
   box16 db '|',13,10,'$'
   box17 db '|',13,10,'$'
   box18 db '|',13,10,'$'
   box19 db '|',13,10,'$'
   box20 db '|',13,10,'$'
   box21 db '|',13,10,'$'
   box22 db '|',13,10,'$'
   box23 db '|',13,10,'$'
   box24 db '|',13,10,'$'
   box25 db '|',13,10,'$'
   box26 db '|',13,10,'$'
   box27 db '|',13,10,'$'
   box28 db '|',13,10,'$'
   box29 db '|',13,10,'$'
   box30 db '|',13,10,'$'
   box31 db '|',13,10,'$'
   box32 db '|',13,10,'$'
   box33 db '|',13,10,'$'
   box34 db '|',13,10,'$'
   box35 db '|',13,10,'$'
   box36 db '|',13,10,'$'
   box37 db '|',13,10,'$'
   box38 db '|',13,10,'$'
   box39 db '|',13,10,'$'
   box40 db '|',13,10,'$'
   box41 db '|',13,10,'$'
   box42 db '|',13,10,'$'
   box43 db '|',13,10,'$'
	
	
	
   
  screen1 db 'Press T for up', 13,10,'$'
  screen2 db 'Press V for down',13,10,'$'
  screen3 db 'Press H for right',13,10,'$'
  screen4 db 'Press D for left',13,10,'$'
  Screen5 db 'Press Q for quit',13,10,'$'
  Name1   db 'By Sharmin Akhter',13,10,'$'
  
  Titl   db "Game of 15", 13,10,'$'
  Line1  db   '1',13,10,'$ ' 
  Line2  db   '5',13,10,'$ '
  Line3  db   '3',13,10,'$'
  Line4  db   '6',13,10,'$'
  Line5  db   '9',13,10,'$ ' 
  Line6  db   '4',13,10,'$ '
  Line7  db   '7',13,10,'$'
  Line8  db   '8',13,10,'$'  
  Line9  db   '2',13,10,'$ ' 
  Line10 db  '14',13,10,'$ '
  Line11 db  '13',13,10,'$'
  Line12 db  '12',13,10,'$' 
  Line13 db  '11',13,10,'$ ' 
  Line14 db  '10',13,10,'$ '
  Line15 db  '15',13,10,'$'
  Line16 db   00h,13,10,'$'
  
  
END start
     
