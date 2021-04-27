# gravor-ashxatanq-of-python
def king_move(x, y, x1, y1):
    if x1 - x == 1 or y1 - y == 1 or x - x1 == 0 or y - y1 == 0:
        print("yes")
    else:
        print("no")
king_move(int(input("input coordinate of x: ")), int(input("input coordinate of y: ")), int(input("input coordinate for move x: ")), int(input("input coordinate for move y: ")))





def sport(x, y):
    z = 0
    while x <= y:
        z += 1
        x += x/10
    return z

print(sport(float(input("input start: ")), float(input("input finish: "))))

def erankyun(a, b, c):
    if a + b > c or a + c > b or c + b > a:
        if a == b and b == c:
            print("havasarakoxm e")
        elif a == b and b != c:
            print("havasarasrun e")
        elif a != b and b != c:
            print("sovorakan erankyun e")
    else:
        print("Hl@ hop tenc erankyun chka")
erankyun(int(input("input a:")), int(input("input b:")), int(input("input c:")))

def hashvich_for_year(days):
    if days % 4 == 0 and days % 100 != 0 or days % 400 == 0:
        print("it is visokosniy")
    else:
        print("it is not visokosni")
hashvich_for_year(int(input("input days: ")))

def chinga_chung(player1, player2):
    player_hashiv1 = 0
    player_hashiv2 = 0
    qar = "qar"
    tuxt = "tuxt"
    mkrat = "mkrat"
    i = 0
    winner = "player_1"
    winner2 = "player_2"
    hashiv = 3
    while i <= hashiv:
        print(player1, player2)
        #qar u tuxt
        if player1 == qar and player2 == tuxt:
           print("The winner is: " + winner2)
        break

        if player2 == qar and player1 == tuxt:
            print("The winner is: " + winner)
        # qar u mkrat

        if player2 == qar and player1 == mkrat:
            print("The winner is: " + winner2)

        elif player2 == mkrat and player1 == qar:
            print("The winner is: " + winner)

        # mkrat u tuxt

        if player2 == tuxt and player1 == mkrat:
            print("The winner is: " + winner)

        elif player2 == mkrat and player1 == tuxt:
            print("The winner is: " + winner2)

chinga_chung(str(input()), str(input()))
