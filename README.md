# saiteja-simplyFy-Question-2

  Assignment 2:
Q . Your son took a vacation through Europe without telling you. When the kid returned from the vacation you asked him where he went. The kid told you: Dad I went to these cities: Amsterdam, Kiev, Zurich, Prague, Berlin, Barcelona.
I used only train as transportation and these were the available tickets:
Paris-Skopje, Zurich-Amsterdam, Prague-Zurich, Barcelona-Berlin, Kiev-Prague, Skopje-Paris, Amsterdam-Barcelona, Berlin-Kiev, Berlin-Amsterdam.
You know that your kid started with Kiev
Write a data structure and algorithm that will give you the route which your son was traveling.


Solution : 
Logic: we can achieve a solution by using a linked data structure here we can consider each station as a node, each node contains the current station and the next station, traveling 1 station to another station we will know the traveling status 
JavaScript Code : 
var head;
class Node {
    constructor(val) {
        this.data = val;
        this.next = null;
    }
}

function printListData() {
    var n = head;
    while (n != null) {
        document.write(n.data + " ");
        n = n.next;
    }
}
var head = new Node('Paris-Skopje');
var second = new Node('Zurich-Amsterdam');
var third = new Node('Prague-Zurich');
var fourth = new Node('Barcelona-Berlin');
var fifth = new Node('Kiev-Prague');
var sixth = new Node('Skopje-Paris');
var seventh = new Node('Amsterdam-Barcelona');
var eighth = new Node('Berlin-Kiev');
var nineth = new Node('Berlin-Amsterdam');
head.next = second;
second.next = third;
third.next = fourth;
fourth.next = fifth;
fifth.next = sixth;
sixth.next = seventh;
seventh.next = eighth;
eighth.next = nineth;
printListData();


