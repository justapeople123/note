# note

# %s字串 %d整數 %f浮點數

#0 None 空 in bool(.)中都是False，非零皆是True

# #一行註解

# """     '''      兩個都是
# """     '''      多行註解

#若一個函數有註解，可用__doc__來取得

#輸入input
#name = input("You name? ") 
#age = int(input("Your age? "))

#使用%
# print ('hello %s, you are %d' % (name, age))  等同 print ('hello, ', name, 'you are ', age)

#使用formatig -> print('hello, {0} you are {1}'.format(name, str(age))) 

#'r'閱讀，'w'撰寫，'a'增加，\n下一行
#盡量多使用'a' ， 'w'有時會覆蓋原本的資料

#s = 'I like python'
#s.lower() 全變小寫
#s.upper() 全變大寫
#s.startswith('I') 是否從I開始
#s.endswith('python') 是否從python結束
#s.isdigit()  是否由數字組成
#s.find('like') 得知like從哪開始，若無此字則回傳-1
#s.replace('like','love') 將like轉為love
#s.split(' ') 以空白為單位來做切割
#s.split(',') 已逗號為單位來做切割

#JOIN
#stooges =['larry','curly','moe']
#' ',join(stooges) 以空白來做合併
#':',join(stooges) 以冒號來做合併
 
#s5 = '0ham and cheesek0'
#s5.strip('0')  去掉頭首

#下面四個都回傳一樣的(使用% OR format)
#'raining %s and %s' % ('cats', 'dogs')
#'raining {} and {}'.format('cats', 'dogs')
#'raining {1} and {0}'.format('dogs', 'cats')
#'raining {arg1} and {arg2}'.format(arg1='cats', arg2='dogs')
#            回傳 'raining cats and dogs'
 
#format
#'pi is {:.2f}'.format(3.14159)  .2f為只要小數點後兩位
#回傳 3.14

#雙引號 and 單引號
#若一段句子裡有單引號，則外圍要使用雙引號"I\'m a pig"
#若有單引號強迫症，可使用'I\'m a pig' 
 
#else if 在Python中是elif

#Python 是透過內縮來判斷區塊的，不是 {}。

#Python 中 else 也可與 while 合用
 
#for loop很常與range搭配使用
#range(5,11,2)
#回傳 5 7 9，從5開始，每2個為一單位，不會觸摸到11(只碰到10，<11的概念)
#break 跳出迴圈 
 
 
 
#Python集合資料
#List:可放不同型態的元素，資料可重複，有順序，可讀可寫。 []
#Tuple:可放不同型態的元素，資料可重複，有順序，只可以讀。 ()
#Set:可放不同型態的元素，資料不可重複，沒有順序，可讀可寫。 aSet = set([12, 23, 34, 'nick']
#Dict:可放不同型態的元素，資料 (key) 不可重複，無順序，由 key, value 組成一個元素。 {}


#List
#兩種方法可以做出空List
#empty_list = []  
#empty_list = list()

#import math
#pow(x,y) 方法返回 x^y（x的y次方） 的值。

#stu = ['nick','kkjj','igr']
#len() 算其長度
#'nick' in stu  回傳True

#weekdays = ['mon', 'tues', 'wed', 'thurs', 'fri'] 
#weekdays[::2] # step = 2 每兩個為一步
#weekdays[::-1] # reverse 倒過來

#students.insert(0, 'maggie') 在ˋ第0的位置加入maggie
#students.remove('nick') 移除nick
#students.pop(2) 移除第 2 位置的值
#del student[0] 移除第 0 位置的值

#students.count('nick') 數出nick在students中的個數
#students.index('albert') 回傳albert在students的位置

#students.sort()  有序排列
#students.sort(reverse = True)  上面的倒過來
#students.sort(key=len)  以字數來有序排列(字短的放前面)
#sorted(students)
#sorted(students, reverse = True)
#sorted(students, key = len)

#加入一個數進入一個已經排序好的數列並讓它也是有序的
#num = [10, 20, 40, 50] 
#from bisect import insort 
#insort(num, 30)
#num
#回傳[10,20,30,40,50]

#num[0] = 0 將第0位置的數改為0
#3種複製list的方法
#num_copy1 = num[:] 
#num_copy2 = list(num) 
#num_copy3 = num.copy()

#num = num2 
#num is num2 回傳True
#num is num_copy1 回傳False(表示指複製其值)

#sorted(list) 與 list.sort() 的不同，前者不會改變 list 的狀態，是回傳另 一個已排序的 list。後者是將 list 做排序，狀態會改
# is 用來檢查是否是相同的參考，== 則用檢查內容是否相同

""""
#變大寫
#fruits = ['apple', 'banana', 'cherry']

#for i in range(len(fruits)):
#    print(fruits[i].upper())

#for fruit in fruits:
#    print(fruit.upper())  結果同上

#for index, fruit in enumerate(fruits):
#    print(index, fruit.upper())  加入index，可出現序號
""""

#for fruit in fruits:
#    if fruit == 'banana':
#        print('I find the banana')
#        break
#else:
#    print("you can't fine the binana")
#若有找到banana，打印並停止，若無，you can't fine the binana


