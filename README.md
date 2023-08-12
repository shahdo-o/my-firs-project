# my-firs-project
arr=[1,2,3,4,5,6,7,8,9]
test=1
def pri(arr):
        print( "@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@\n@             @             @             @\n"
        
        
             "|     ",arr[0],"     |     " ,arr[1],"     |     " ,arr[2],"     |     ","\n\n"
             "@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@\n@             @             @             @\n"
             
             
             "|     ",arr[3],"     |     " ,arr[4],"     |     " ,arr[5],"     |     ","\n\n"
             "@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@\n@             @             @             @\n"
             
             
             "|     ",arr[6],"     |     " ,arr[7],"     |     " ,arr[8],"     |     ","\n\n"
             "@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@")
def game(num,name):
      global test
      num =num-1
      if arr[0]==arr[1] and arr[0]==arr[2]:
            print("the winner is " , name)
            test=0
           
    
      elif arr[5]==arr[3]and arr[3]==arr[4]:
            print("the winner is " ,  name)
            test=0
            
    
      elif arr[8]==arr[6] and arr[8]==arr[7]:
        pri(arr)
        print("the winner is " ,  name)
        test=0
        
    
      elif arr[0]==arr[3] and arr[3]==arr[6]:
        pri(arr)
        print("the winner is" ,  name)
        test=0
        
      elif arr[1]==arr[4] and arr[4]==arr[7]:
        pri(arr)
        print("the winner is" ,  name)
        test=0
        
      elif arr[2]==arr[5] and arr[5]==arr[8]:
        pri(arr)
        print("the winner is" ,  name)
        test=0
        
      elif arr[0]==arr[4] and arr[4]==arr[8]:
        pri(arr)
        print("the winner is" ,  name)
        test=0
        
      elif arr[2]==arr[4] and arr[4]==arr[6]:
        pri(arr)
        print("the winner is" ,  name)
        test=0
        
   
def play1():
       pri(arr)
       print(n_player1,":")
       f= int (input( " choose num 1:9 ??  "))
       if arr[f-1]==player2 or arr[f-1]==player1 or 9<f<0:
            play1 ()
       else:
             arr[f-1]= player1
             game(f,n_player1)
                
def play2():
       pri(arr)
       print(  n_player2,":")
       f= int (input("choose num 1:9 ??  "))
       if arr[f-1]==player2 or arr[f-1]==player1 or 9<f<0:
            play2 ()
       else:
             arr[f-1]= player2
             game(f,n_player2)             

print ('''******************************************************************     
               **************   (Welcome to the game)    **********
                            ******************************''')



player1=""
player2 =""
def log ():
        global n_player1 , n_player2 ,player1, player2
        p=input("choose x or y ").lower()

        if p=="x":
            player1="x"
            player2="y"
            n_player1=input("Please write your name:   ")   
            n_player2=input("Please write the competitor's name :  ") 
        elif p=="y" :
                player2="x"
                player1="y"
                n_player1=input("Please write your name:   ")   
                n_player2=input("Please write the competitor's name :  ") 
        else :
                print("error")
                log ()
          

log()
while (test):
       
       play1()
       if (test== 1):
           play2()
            
