CXX = c++

CXXFLAGS = -Wall -Wextra -Werror -std=c++98

TARGET = maintrace

SRCS = main.cpp Animal.cpp Cat.cpp Dog.cpp WrongCat.cpp WrongAnimal.cpp

OBJS = $(SRCS:.cpp=.o)

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CXX) $(OBJS) -o $(TARGET)

%.o: %.cpp
	$(CXX) $(CXXFLAGS) -c $< -o $@

clean:
	rm -f $(OBJS) 

fclean: clean
	$(RM) $(NAME) $(TARGET)

re: fclean all

.PHONY: all clean fclean re
