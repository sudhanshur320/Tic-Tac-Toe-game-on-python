# Tic-Tac-Toe-game-on-python
It is a very popular Tic-Tac-Toe game developed on python.









board={"T1": " ","T2": " ","T3": " ",
       "M1": " ","M2": " ","M3": " ",
       "D1": " ","D2": " ","D3": " "}

player=1                              # to initialize first player
total_moves=0                         # to count the moves

print("T1|T2|T3")
print("--|--|--")
print("M1|M2|M3")
print("--|--|--")
print("D1|D2|D3")
print()
print("************************************")
print()
print()

while True:
    print(board["T1"]+"|"+board["T2"]+"|"+board["T3"])
    print("-|-|-")
    print(board["M1"]+"|"+board["M2"]+"|"+board["M3"])
    print("-|-|-")
    print(board["D1"]+"|"+board["D2"]+"|"+board["D3"])
    if total_moves==9:
        break
    while True:                          #input from players
        if player==1:                    # choose player
            p1=input("palyer one  :  ")
            if p1.upper() in board and board[p1.upper()]==" ":
                board[p1.upper()]="X"
                player=2
                break     
            else:                           # on wrong input
                print("Invalid Input , please try again")
                continue        
        else:
             if player==2:                    # choose player
                    p2=input("palyer two  :  ")
                    if p2.upper() in board and board[p2.upper()]==" ":
                        board[p2.upper()]="O"
                        player=1
                        break
                    else:                     # on wrong input
                        print("Invalid Input , please try again")
                        continue                    
    total_moves=total_moves+1
    print("************************************")
    print()
                        
    
            
    
