# -Independent-

def show_mesage(text: str) -> str:
    """Find a hided message"""
    m = []
    for i in text:
      if i.isupper():
        m.append(i)  
        text = "".join(m)
      elif text.islower():
        text = ""
    return text
      
if __name__ == '__main__':
    print('Example:')
    print(show_mesage("How are you? Eh, ok. Low or Lower? Ohhh."))
    assert show_mesage("How are you? Eh, ok. Low or Lower? Ohhh.") == "HELLO", "hello"
    assert show_mesage("hello world!") == "", "Nothing"
    assert show_mesage("HELLO WORLD!!!") == "HELLOWORLD", "Capitals"
    print("Cool")
