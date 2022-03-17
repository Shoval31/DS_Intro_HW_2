# DS_Intro_HW_2
def reverse(sentence, reverse_word):
    try:
        type(sentence) == str
        type(reverse_word) == str
        count = sentence.count(reverse_word) #1
        if count == 0:
            print("could not find the word")
        else:
            x = sentence.find(reverse_word)
            new_word = reverse_word[::-1]
            new_sentence = sentence[:x]+new_word+sentence[x+len(new_word):]
            print(new_sentence)            
    except:
      print("input error detected")
