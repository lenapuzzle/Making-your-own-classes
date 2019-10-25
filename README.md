# Making-your-own-classes


using System;

namespace Color
{
    class Program
    {
        static void Main(string[] args)
        {

            Console.ReadLine();
        }
    }
    class Color
    {
        private byte red;
        private byte blue;
        private byte green;
        private byte alpha;

        public Color(byte red, byte blue, byte green, byte alpha)
        {
            this.red = red;
            this.blue = blue;
            this.green = green;
            this.alpha = alpha;
        }

        public Color(byte red, byte blue, byte green)
        {
            this.red = red;
            this.blue = blue;
            this.green = green;
            this.alpha = 255;
        }

        public byte GetRed()
        {
            return red;
        }

        public void SetRed(byte red)
        {
            this.red = red;
        }

        public byte GetBlue()
        {
            return blue;
        }

        public void SetBlue(byte blue)
        {
            this.blue = blue;
        }

        public byte GetGreen()
        {
            return green;
        }

        public void SetGreen(byte green)
        {
            this.green = green;
        }

        public byte GetAlpha()
        {
            return alpha;
        }

        public void SetAlpha(byte alpha)
        {
            this.alpha = alpha;
        }

        public byte GetGrayscale()
        {
            return (byte)((red + blue + green) / 3);
        }
    }   
}
