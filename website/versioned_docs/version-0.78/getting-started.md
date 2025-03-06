import React from "react";
import { View, Text, TextInput, TouchableOpacity } from "react-native";
import { Ionicons } from "@expo/vector-icons";

const HomeScreen = () => {
  return (
    <View style={{ flex: 1, padding: 20, backgroundColor: "#f8f8f8" }}>
      
      {/* Header */}
      <Text style={{ fontSize: 24, fontWeight: "bold", marginBottom: 20 }}>
        🏪 Supermercato Finder
      </Text>
      
      {/* Barra di Ricerca */}
      <View style={{ flexDirection: "row", alignItems: "center", backgroundColor: "#fff", padding: 10, borderRadius: 10, shadowColor: "#000", shadowOpacity: 0.1, shadowRadius: 5 }}>
        <Ionicons name="search" size={20} color="#888" />
        <TextInput
          placeholder="Cerca un prodotto..."
          style={{ marginLeft: 10, flex: 1 }}
        />
      </View>
      
      {/* Icone Navigazione */}
      <View style={{ flexDirection: "row", justifyContent: "space-around", marginTop: 30 }}>
        <TouchableOpacity>
          <Ionicons name="map" size={50} color="#007bff" />
          <Text style={{ textAlign: "center", marginTop: 5 }}>Mappa</Text>
        </TouchableOpacity>

        <TouchableOpacity>
          <Ionicons name="cart" size={50} color="#28a745" />
          <Text style={{ textAlign: "center", marginTop: 5 }}>Lista</Text>
        </TouchableOpacity>

        <TouchableOpacity>
          <Ionicons name="pricetag" size={50} color="#ff5733" />
          <Text style={{ textAlign: "center", marginTop: 5 }}>Offerte</Text>
        </TouchableOpacity>
      </View>
    </View>
  );
};

export default HomeScreen;

