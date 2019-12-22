# Think-out-of-BOX
Always try not to be satisfied with your'e code, which will make you a good developer.
from PyQt5 import QtGui,QtWidgets
from PyQt5.QtWidgets import QApplication, QMainWindow, QLabel
from PyQt5.QtGui import QPixmap, QIcon
from PyQt5.QtCore import Qt, pyqtSignal, QTimer
import sys
import os
from OtherWindow import Ui_OtherWindow

class Window(QMainWindow):
    global x
    global image
    i='1'
    while True:
        print("running")
        f=open("comd.txt")
        x=f.read()
        if(x!=""):
            f=open("comd.txt",'w').close
            break
    image=[]
    image.append("qwer")
    while True: 
            if(os.path.exists(x+i+".jpeg")==True):
                image.append(x+i)
                i=int(i)
                i=i+1
                i=str(i)
                print(i)
        
            else:
                break
    print(image)
    def __init__(self):
        super().__init__()

        self.title = "PyQt Image"
        self.top = 100
        self.left = 100
        self.width = 680
        self.height = 500
        self.InitWindow()
    def pp1(self,event):
        f=open("det.txt",'w')
        f.write(x+'1')
        f.close()
        print(event)
        self.window = QtWidgets.QMainWindow()
        self.ui=Ui_OtherWindow()
        self.ui.setupUi(self.window)
        self.window.show()

    def pp2(self,event):
        f=open("det.txt",'w')
        f.write(x+'2')
        f.close()
        print(event)
        self.window = QtWidgets.QMainWindow()
        self.ui=Ui_OtherWindow()
        self.ui.setupUi(self.window)
        self.window.show()

    def pp3(self,event):
        f=open("det.txt",'w')
        f.write(x+'3')
        f.close()
        print(event)
        self.window = QtWidgets.QMainWindow()
        self.ui=Ui_OtherWindow()
        self.ui.setupUi(self.window)
        self.window.show()

    def pp4(self,event):
        f=open("det.txt",'w')
        f.write(x+'4')
        f.close()
        print(event)
        self.window = QtWidgets.QMainWindow()
        self.ui=Ui_OtherWindow()
        self.ui.setupUi(self.window)
        self.window.show()

    def pp5(self,event):
        f=open("det.txt",'w')
        f.write(x+'5')
        f.close()
        print(event)
        self.window = QtWidgets.QMainWindow()
        self.ui=Ui_OtherWindow()
        self.ui.setupUi(self.window)
        self.window.show()

    def pp6(self,event):
        f=open("det.txt",'w')
        f.write(x+'6')
        f.close()
        print(event)
        self.window = QtWidgets.QMainWindow()
        self.ui=Ui_OtherWindow()
        self.ui.setupUi(self.window)
        self.window.show()

    def pp7(self,event):
        f=open("det.txt",'w')
        f.write(x+'7')
        f.close()
        print("hello")
        print(event)
        self.window = QtWidgets.QMainWindow()
        self.ui=Ui_OtherWindow()
        self.ui.setupUi(self.window)
        self.window.show()

    def pp8(self,event):
        f=open("det.txt",'w')
        f.write(x+'8')
        f.close()        
        print("hello")
        print(event)
        self.window = QtWidgets.QMainWindow()
        self.ui=Ui_OtherWindow()
        self.ui.setupUi(self.window)
        self.window.show()

    def InitWindow(self):
        self.label1 = QLabel(self)
        try:
            self.pixmapImage = QPixmap(image[1]+".jpeg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        except:
            self.pixmapImage = QPixmap("winners.jpg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        self.label1.setPixmap(self.pixmapImage)
        self.label1.setGeometry(15,15,120,130)
        self.label1.mousePressEvent = self.pp1

        self.label2 = QLabel(self)
        try:
            self.pixmapImage = QPixmap(image[2]+".jpeg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        except:
            self.pixmapImage = QPixmap("winners.jpg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        self.label2.setPixmap(self.pixmapImage)
        self.label2.setGeometry(175,15,118,130)
        self.label2.mousePressEvent = self.pp2

        self.label3 = QLabel(self)
        try:
            self.pixmapImage = QPixmap(image[3]+".jpeg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        except:
            self.pixmapImage = QPixmap("winners.jpg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        self.label3.setPixmap(self.pixmapImage)
        self.label3.setGeometry(340,15,118,130)
        self.label3.mousePressEvent = self.pp3

        self.label4 = QLabel(self)
        try:
            self.pixmapImage = QPixmap(image[4]+".jpeg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        except:
            self.pixmapImage = QPixmap("winners.jpg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        self.label4.setPixmap(self.pixmapImage)
        self.label4.setGeometry(505,15,118,130)
        self.label4.mousePressEvent = self.pp4

        self.label5 = QLabel(self)
        try:
            self.pixmapImage = QPixmap(image[5]+".jpeg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        except:
            self.pixmapImage = QPixmap("winners.jpg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        self.label5.setPixmap(self.pixmapImage)
        self.label5.setGeometry(15,175,118,130)
        self.label5.mousePressEvent = self.pp5

        self.label6 = QLabel(self)
        try:
            self.pixmapImage = QPixmap(image[6]+".jpeg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        except:
            self.pixmapImage = QPixmap("winners.jpg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        self.label6.setPixmap(self.pixmapImage)
        self.label6.setGeometry(175,175,118,130)
        self.label6.mousePressEvent = self.pp6

        self.label7 = QLabel(self)
        try:
            self.pixmapImage = QPixmap(image[7]+".jpeg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        except:
            self.pixmapImage = QPixmap("winners.jpg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        self.label7.setPixmap(self.pixmapImage)
        self.label7.setGeometry(340,175,118,130)
        self.label7.mousePressEvent = self.pp7

        self.label8 = QLabel(self)
        try:
            self.pixmapImage = QPixmap(image[8]+".jpeg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        except:
            self.pixmapImage = QPixmap("winners.jpg").scaled(112,128,Qt.KeepAspectRatio,Qt.SmoothTransformation)
        self.label8.setPixmap(self.pixmapImage)
        self.label8.setGeometry(505,175,118,130)
        self.label8.mousePressEvent = self.pp8

        
        self.setWindowTitle(self.title)
        self.setGeometry(self.top,self.left,self.width,self.height)
        self.show()

App = QApplication(sys.argv)
window = Window()
sys.exit(App.exec())
