people = {
    'Alice':{
        'phone':'2341',
        'addr':'Foo drive 23'
    },
    'Beth':{
        'phone':'9102',
        'addr':'Bar street 42'
    },
    'Cecil':{
        'phone':'3158',
        'addr':'Baz avenue 90'
    }

}
labels = {
    'phone':'phone number',
    'addr':'address'
}
name= input('name:')
request = input('phone number (p) or address(a)?')
if request ==  'p' : key = 'phone'
if request ==  'a' : key = 'addr'
if name in people: print("{}'s {} is {}.".format(name,labels[key],people[name][key]))
