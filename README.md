# Python-Projects
print("Good Morning Everyone!!! WELCOME TO MY PYTHON PROJECT")
print("My Name Is Adityan \nRegisteration Number:- 12216198")

N=int(input("Enter the number of pieces you want to cut the cake into: ")) #N is the number of pieces in which the cake needs to be divided.
A=360/N
if 360%N==0:
    print("---> YES the cake will cut in equal pieces of appropriate angle", A,"degrees")
else:
    print('''---> NO the cake will not cut in equal pieces of same appropriate angle
because in that case the appropriate angle of each piece of cake will be''',A, '''degrees and
it has already been given that the appropriate angle of the cake must be an integer''')
if(N<=360):
    print("---> YES the cake will cut into",N ,"pieces")
else:
    print("---> NO the cake will cut into",N ,"pieces")

b=int(A-(N/2))
g=int(A+(N/2)) 
c=int(360//N)     
d=N-1
if 360%N==0:
    if b>0:
        print("---> Yes the cake will cut into" ,N ,"pieces such that no two of them are equal")
    else:
        print("---> NO the cake will not cut into" ,N ,"pieces such that no two of them are equal")
else:
    if c-(d/2)>=2 and d<(c+(d/2)):
        print("---> Yes the cake will cut into" ,N ,"pieces such that no two of them are equal")
    elif c-(d/2)<2 and d<(c+(d/2)):
        print("---> NO the cake will not cut into" ,N ,"pieces such that no two of them are equal")
    elif c-(d/2)<1:
        print("---> NO the cake will not cut into" ,N ,"pieces such that no two of them are equal")
    elif c-(d/2)>=1 and d>(c+(d/2)):
        print("---> Yes the cake will cut into" ,N ,"pieces such that no two of them are equal")
print("THANK YOU")
    
#EXPLANATION FOR THE CODE

'''360/10=36
that is ONE OF THE POSSIBLE COMBINATION OF APPROPRIATE ANGLE FOR 10 PIECES  OF CAKE IS 31,35,37,34,38,33,39,32,40,41

360/20=18
that is ONE OF THE POSSIBLE COMBINATION OF APPROPRIATE ANGLE FOR 20 PIECES  OF CAKE IS 8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28

360/24=15
that is ONE OF THE POSSIBLE COMBINATION OF APPROPRIATE ANGLE FOR 24 PIECES  OF CAKE IS 3,4,5,6,7,8,9,10,11,12,13,14,16,17,18,19,20,21,22,23,24,25,26,27

360/25=14.4
that is 14*24 + 24
that is ONE OF THE POSSIBLE COMBINATION OF APPROPRIATE ANGLE FOR 24 PIECES  OF CAKE IS 2,3,1,5,6,7,8,9,10,11,12,13,15,16,17,18,19,20,21,22,23,27,25,26,24

360/26=13.846
that is 13*25 + 35
that is ONE OF THE POSSIBLE COMBINATION OF APPROPRIATE ANGLE FOR 24 PIECES  OF CAKE IS 1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25

360/27=13.333
that is 13*26 + 22
In this case we can see that c-(d/2)=13-(26/2)=0. So the number of possible combinations of appropriate angle for 26 pieces of cake will never be all different.
'''

