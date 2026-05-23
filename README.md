import streamlit as st
st.title('Strong Motors - Aluguel de Carros')
st.sidebar.title('Escolha Seu Modelo')
st.sidebar.image('logo.png')

carros = ['Escolha o Carro','BMW i7','Cybertruck','Fusca','FIAT Toro','Lamborghini Veneno','Lamborghini Centenario','Lamborghini Aventador']

opcao = st.sidebar.selectbox('Escolha o carro alugado', carros)

st.image(f'{opcao}.png')
st.markdown(f'## Você alugou o modelo: {opcao}')
st.markdown('---')

dias = st.text_input(f'Por quantos dias o {opcao} foi alugado?')
km = st.text_input(f'quantos KM você rodou com o {opcao}?')
