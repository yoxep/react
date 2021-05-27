# react
import React from 'react';
import { StyleSheet, Text, View, Image,ScrollView } from 'react-native';
import Honeytitip from "./assets/Honeytitip.png"
import pizza from "./assets/pizza.png"



export default function App() {
  return (
      <View style={styles.container}>
        <Text style={styles.naman}>나만의 ddkdk꿀팁</Text>
        <Text></Text>
          <Image 
        source={Honeytitip}
            // 사용설명서에 나와 있는 resizeMode 속성 값을 그대로 넣어 적용합니다
        resizeMode={"cover"}
        style={styles.imageStyle}
          />
         <Text></Text>
      <ScrollView style={styles.ee}
      horizontal={true}>
        
      <View style={styles.textContainer1}>
        <Text style={styles.textStyle}>미용</Text>
      </View>
      <View style={styles.textContainer2}>
        <Text style={styles.textStyle}>재테크</Text>
      </View>
      <View style={styles.textContainer3}>
        <Text style={styles.textStyle}>할인</Text>
      </View>
      <View style={styles.textContainer4}>
        <Text style={styles.textStyle}>음식</Text>
      </View>
      </ScrollView>

    <View style={styles.downbu}>
      
      <Image 
        source={pizza}
            // 사용설명서에 나와 있는 resizeMode 속성 값을 그대로 넣어 적용합니다
        resizeMode={"cover"}
        style={styles.pizzaimageStyle2}
          />
        
      </View>

      </View>
      
    );
};

const styles = StyleSheet.create({
  container: {
    padding:15,
    marginTop: 30,
    marginLeft: 10,
    marginRight: 10,
    flex:1,
    flexDirection:'column'
  },
  ee:{
    flex:2,
    
  },
  textContainer1: {
    height:60,
    width:100,
    backgroundColor:'#ffe650',
    borderColor:'#ffe650',
    borderWidth:2,
    borderRadius:10,
    margin:10,
    padding:10,
  },
  textContainer2: {
    height:60,
    width:100,
    backgroundColor:'#ffd4df',
    borderColor:'#ffd4df',
    borderWidth:2,
    borderRadius:10,
    margin:10,
    padding:10,
  },
  textContainer3: {
    height:60,
    width:100,
    backgroundColor:'#fd93f9',
    borderColor:'#fd93f9',
    borderWidth:2,
    borderRadius:10,
    margin:10,
    padding:10,
  },
  textContainer4: {
    height:60,
    width:100,
    backgroundColor:'rgb(214,122,127)',
    borderColor:'rgb(214,122,127)',
    borderWidth:2,
    borderRadius:10,
    margin:10,
    padding:10,
  },
  imageStyle: {
    flex:3,
    borderRadius:15,
    height:'30%',
    width:'100%',
    alignItems:"center",
    justifyContent:"center"
  },
  pizzaimageStyle2: {
    borderRadius:10,
    height:'30%',
    width:'40%',
    alignItems:"center",
    justifyContent:"center"
  },

  downbu:{
    flex:4,
    
  },

  naman: {
    
    color: 'black',
    fontWeight: 'bold',
    fontSize: 25,
    
  },
});
