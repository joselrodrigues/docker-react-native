FROM node:12

EXPOSE 19000
EXPOSE 19001
EXPOSE 19002
EXPOSE 19006

WORKDIR /usr/src/app
COPY . .
WORKDIR /usr/src/app/ReactNative

#install latest yarn
RUN curl --compressed -o- -L https://yarnpkg.com/install.sh | bash
#Add expo-cli globaly
RUN yarn global add expo-cli
#install all react-native dependencies
RUN yarn install
CMD yarn start