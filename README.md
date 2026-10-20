


Class_name = {}
list = []
while True:
    menu = input("1.add 2.delete 3.show: ")
    match menu:
        case"1":
            kode_class = int(input("kode class vared kon:"))
            teacher_name = input("name teachereto vared kon: ")
            class_name = int(input("shomare kelaseto vared kon:"))
            roz = (input("che rozi:"))
                      
            Class_name[kode_class] = {"teacher_name": teacher_name,"class_name": class_name,"roz": roz}
        
            print(Class_name)
        case "2":
            kode_class = int(input("kode class baraye hazf: "))
            if kode_class in Class_name:
                Class_name.pop(kode_class)
                print(Class_name)
            else:
                print("nadarim")
        case "3":
            print(Class_name)
            break
