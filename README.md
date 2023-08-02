# number-cardgame
숫자 카드게임은 여러개의 숫자중에서 가장 큰 숫자가 쓰인 카드 한장을 뽑는다.
행과 열이 입력 되면  행과 열에 각 숫자를 입력받는다.
선택된 행의 카드중에서 가장 낮은 숫자 뽑을 수 있다는 것을 고려해서 최종적으로는 가장 높은 숫자의 카드를 뽑게 전략을 세워라. --> '각 행에서 뽑은 낮은 숫자의 카드들을 찾은 후에 그중에서 가장 큰 수를 찾아라!'
#python code

N,M=map(int,input().split())
data=0
for i in range(N):
    cards=list(map(int,input().split())) #각행마다의 카드수를을 받음 
    small=min(cards)
    #각 행중의 가장 작은 수를 저장 
    data=max(data,small)
    #저장된수중에서 가장 큰 수를 확인 
print(data)
